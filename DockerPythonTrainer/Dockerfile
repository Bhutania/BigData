FROM rocm/tensorflow:rocm3.3-tf1.13-centos-mkl-dev
LABEL maintianer="Tyler Cole"

ENV CENTOS_FRONTEND noninteractive

ADD Keras-CoDeepNEAT /Keras-CoDeepNEAT
ADD run_mnist.py /run_mnist.py

RUN yum install -y python3.6-dev graphviz* libgraphviz-dev  

RUN pip install kafka-python
RUN pip install -Iv keras==2.2.5
RUN pip install -Iv networkx==2.3
RUN pip install -Iv pydot==1.4.1
RUN pip install graphviz
RUN pip install pygraphviz
RUN pip install sklearn
RUN pip install matplotlib==3.2.1



ENTRYPOINT ["python3",  "/run_mnist.py"]

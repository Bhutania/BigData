FROM rocm/tensorflow:rocm3.3-tf1.13-centos-mkl-dev
LABEL maintianer="Tyler Cole"


ENV CENTOS_FRONTEND noninteractive

ADD app.py /app.py

RUN pip3 install kafka-python
RUN pip3 install keras
RUN pip3 install networkx


ENTRYPOINT ["python3",  "/app.py"]

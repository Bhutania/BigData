FROM rocm/tensorflow:latest
LABEL maintianer="Tyler Cole"


ENV DEBIAN_FRONTEND noninteractive

ADD app.py /app.py

RUN pip3 install kafka-python
RUN pip3 install keras
RUN pip3 install networkx


ENTRYPOINT ["python3",  "/app.py"]

FROM python:2.7
ENV PYTHONUNBUFFERED 1
RUN mkdir /code
WORKDIR /code
ADD requirements.txt /code/
RUN apt-get update && apt-get install python-dev libmysqlclient-dev -y
RUN pip install -r requirements.txt
ADD . /code/

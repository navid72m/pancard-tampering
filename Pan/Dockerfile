# syntax=docker/dockerfile:1

FROM python:3.8-slim-buster

WORKDIR /python-docker

COPY requirements.txt /python-docker/requirements.txt
RUN pip3 install -r requirements.txt

COPY . /python-docker

CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]

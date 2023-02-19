FROM python:3.11-buster

RUN mkdir app
WORKDIR /app

ENV="${PATH}:/root/.local/bin"
ENV PYTHONPATH=.

COPY requirements.txt .
RUN pip install --upgrade pip
RUN pip isntall -r requirements.txt

COPY src/ .
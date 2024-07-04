FROM python:3.10

LABEL maintainer="backendimg"

ENV PYTHONUNBUFFERED 1

WORKDIR /backend

# Instala postgresql-client
RUN apt-get update && apt-get install -y git cron

COPY ./app/requirements.txt /backend/
RUN pip install -r requirements.txt

COPY ./app/* /backend/
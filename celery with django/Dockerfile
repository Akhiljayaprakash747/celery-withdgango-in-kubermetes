FROM python:3.6-slim
MAINTAINER Mark Gituma <mark.gituma@gmail.com>

ENV PROJECT_ROOT /app
WORKDIR $PROJECT_ROOT

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN /usr/local/bin/python -m pip install --upgrade pip
COPY . .
CMD python manage.py runserver 0.0.0.0:8000

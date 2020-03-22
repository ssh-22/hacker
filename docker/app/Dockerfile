FROM python:3.8.2

ENV PYTHONUNBUFFERED 1

WORKDIR /app

COPY . .

RUN pip install --upgrade pip
RUN pip install poetry

WORKDIR /app/app

RUN poetry config virtualenvs.create false \
  && poetry install

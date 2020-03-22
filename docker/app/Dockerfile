FROM python:3.8.2

ENV PYTHONUNBUFFERED 1

COPY . .

WORKDIR /app

RUN pip install --upgrade pip
RUN pip install poetry

RUN poetry config virtualenvs.create false \
  && poetry install

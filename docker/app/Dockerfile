FROM python:3.8.2

ENV PYTHONUNBUFFERED 1

WORKDIR /src

COPY . .

RUN pip install --upgrade pip
RUN pip install poetry

WORKDIR /src/src

RUN poetry config virtualenvs.create false \
  && poetry install

FROM python:3.10-slim

WORKDIR /app

COPY Pipfile /app/

RUN pip install pipenv && \
    pipenv install --system

COPY . /app

EXPOSE 5000

CMD ["python", "app.py"]

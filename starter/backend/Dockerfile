FROM python:3.10-slim

WORKDIR /app

COPY Pipfile Pipfile.lock /app/

RUN pip install pipenv && \
    pipenv install --system --deploy

COPY . /app

EXPOSE 5000

CMD ["python", "app.py"]

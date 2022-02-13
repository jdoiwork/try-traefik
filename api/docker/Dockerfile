FROM python:3.10

COPY requirements.txt /tmp/requirements.txt

RUN pip install -r /tmp/requirements.txt

EXPOSE 80

# COPY ./app /app

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80", "--root-path", "/api"]
# CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]

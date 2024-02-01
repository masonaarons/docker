# This file will contain all of the instructions for how docker will package your container in an image and run it
FROM python:3.9.12-buster
# Base image

ENV FLASK_ENV='development'
ENV FLASK_APP='app.py'

WORKDIR /app

COPY . .

RUN pip install -r requirements.txt

CMD ["python", "-m", "flask", "run", "--host=0.0.0.0"]

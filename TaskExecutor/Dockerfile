FROM python:3.12 as builder
LABEL author="Igor Walkowiak"

WORKDIR /app
COPY requirements.txt /app
RUN target=/root/.cache/pip pip3 install -r requirements.txt

COPY ./src /app
CMD [ "python3", "-m" , "flask", "run", "-h", "0.0.0.0"]

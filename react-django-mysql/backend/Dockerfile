FROM python:3.7

WORKDIR /app/backend
COPY requirements.txt /app/backend
RUN pip3 install --upgrade pip -r requirements.txt

COPY . /app/backend
EXPOSE 5000

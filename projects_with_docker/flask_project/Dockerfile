FROM ubuntu:18.04
RUN apt-get update -y
RUN apt-get install -y python3-pip python3-dev build-essential 
RUN mkdir /FlaskApp
WORKDIR /FlaskApp
COPY ./requirements.txt .
RUN pip3 install -r requirements.txt
COPY ./ ./
EXPOSE 8000
CMD ["python3", "hello.py"]


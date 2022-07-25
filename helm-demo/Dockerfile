FROM python:3.9-slim-buster

RUN  pip3 --version;

EXPOSE 8000

RUN mkdir myapp
COPY DevOps-Challenge ./app
WORKDIR /app
RUN pip3 install -r requirements.txt

# redis port 
EXPOSE 6379 

ENTRYPOINT ["/bin/bash" , "-c", "export $(cat .env | xargs) && python hello.py"]
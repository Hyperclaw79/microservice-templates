FROM python:3.7.0a3-alpine3.7

WORKDIR /deploy

COPY requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt

COPY deploy.py /deploy/deploy.py

COPY config.json /deploy/config.json

COPY functions /deploy/functions

CMD ["python", "deploy.py"]

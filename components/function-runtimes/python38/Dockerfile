# kubeless/python:3.7
FROM python:3.8.8-alpine3.13

LABEL source = git@github.com:kyma-project/kyma.git

RUN pip install bottle==0.12.13 cherrypy==8.9.1 wsgi-request-logger==0.4.6 prometheus_client==0.8.0

COPY kubeless/ /

WORKDIR /

USER 1000

CMD ["python", "/kubeless.py"]

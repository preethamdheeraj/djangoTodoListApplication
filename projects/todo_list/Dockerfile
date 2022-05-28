FROM python:3.10-alpine

ENV PATH = "/scripts:${PATH}"

COPY ./requirements.txt /requirements.txt
RUN apk add --update --no-cache --virtual .tmp gcc libc-dev linux-headers
# apk is the alpine package manager command
RUN pip install -r /requirements.txt
RUN apk del .tmp

RUN mkdir /todo_projects
COPY ./todo_projects /todo_projects
WORKDIR /todo_projects
COPY ./scripts /scripts

RUN chmod +x /scripts/*

RUN mkdir -p /vol/web/media     
RUN mkdir -p /vol/web/static
# created for the future if the user will be updating files in the django application 


CMD ["/scripts/entrypoint.sh"]


# Set the base image
FROM python:3.6

# Dockerfile author / maintainer
MAINTAINER Matheus Mota <docker@matheusmota.com>

RUN apt-get update
RUN apt-get upgrade -y


WORKDIR /jup

# installing jupyer + jupyterlab
RUN pip install jupyter -U && pip install jupyterlab

#Exposing default port
EXPOSE 8888

ENTRYPOINT ["jupyter", "lab","--ip=0.0.0.0","--allow-root"]


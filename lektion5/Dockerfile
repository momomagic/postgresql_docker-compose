FROM jupyter/scipy-notebook
USER root
RUN apt-get update
RUN apt-get install -y libpq-dev
COPY requirements.txt /opt/requirements.txt
RUN pip install -r /opt/requirements.txt
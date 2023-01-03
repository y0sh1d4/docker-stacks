# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
ARG BASE_CONTAINER=minimal-notebook-gpu
FROM $BASE_CONTAINER

USER root
RUN     apt update && \
        apt install -y \
        libopencv-dev\
        opencv-data

ADD requirements.txt .
RUN pip install --upgrade pip &&\
	pip install -r requirements.txt -U
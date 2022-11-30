# syntax=docker/dockerfile:1
FROM nvidia/cuda:11.6.2-base-ubuntu20.04
FROM tensorflow/tensorflow:latest-gpu-jupyter

COPY requirements.txt .
RUN apt-get update
RUN python3 -m pip install --upgrade pip
RUN pip install -r requirements.txt
WORKDIR /workspace/
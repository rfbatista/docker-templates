FROM ubuntu:18.04

WORKDIR /app

RUN apt-get update && apt-get install -y software-properties-common gcc && \
    add-apt-repository -y ppa:deadsnakes/ppa

RUN apt-get update && apt-get install -y python3.6 python3-distutils python3-pip python3-apt

# Install dependencies
RUN apt-get update && apt-get install python3-pip

RUN pip3 install --upgrade pip

RUN pip3 install --no-cache-dir -U  sentence-transformers
# Copies script.py file in my current directory to root in the container
# COPY similarity.py .

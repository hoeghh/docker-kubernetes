FROM ubuntu:20.04

RUN apt-get update && apt-get install -y curl \
  && rm -rf /var/lib/apt/lists/*

ENV MEDUSA_VERSION=0.2.0

RUN useradd -ms /bin/bash ubuntu
WORKDIR /home/ubuntu
USER ubuntu

RUN curl -L https://github.com/jonasvinther/medusa/releases/download/v0.2.0/medusa_0.2.0_linux_amd64.tar.gz -o medusa.tar.gz
RUN ls -l

RUN tar xvf medusa.tar.gz

RUN ls -l

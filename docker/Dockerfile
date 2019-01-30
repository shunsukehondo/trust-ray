FROM ubuntu:18.04

COPY ./entrypoints /entrypoints

WORKDIR /opt/server

RUN apt-get update && apt-get install -y build-essential curl git make
RUN curl -sL https://deb.nodesource.com/setup_6.x | bash -
RUN apt-get update && apt-get install -y nodejs npm

CMD /entrypoints/run

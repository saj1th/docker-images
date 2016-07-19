FROM debian:8.5

MAINTAINER Sajith Appukuttan <asajith@gmail.com>

ENV LANG=C.UTF-8 LC_ALL=C.UTF-8

RUN apt-get update --fix-missing && apt-get install -y curl sudo
RUN curl -sL https://deb.nodesource.com/setup | sudo bash -
RUN apt-get -y install nodejs
RUN apt-get -y install build-essential
RUN npm install -g kinesalite

EXPOSE 4567

ENTRYPOINT ["/usr/bin/kinesalite"]

CMD ["--help"]

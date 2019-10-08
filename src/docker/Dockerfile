FROM ruby:alpine
MAINTAINER Radu Helstern <radu.helstern@gmail.com>

RUN apk add --no-cache build-base git && \
    gem install travis && \
    gem install travis-lint && \
    gem install travis-conditions && \
    apk del build-base &&\
    mkdir project

WORKDIR project

VOLUME ["/project"]

ENTRYPOINT ["travis"]
FROM ruby:2.7-alpine
MAINTAINER Brian Rutledge "bhrutledge@gmail.com"

RUN set -ex \
    && apk add --update --no-cache --virtual build-dependencies \
        build-base \
        ruby-dev \
        libffi-dev \
    && gem install --no-document \
        json \
        compass \
    && apk del build-dependencies

ENTRYPOINT ["compass"]

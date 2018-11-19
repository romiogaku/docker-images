FROM node:10-alpine

RUN apk -v --update add \
  make \
  gcc \
  g++ \
  zip \
  python \
  py-pip \
  groff \
  less \
  mailcap \
  zlib-dev \
  autoconf \
  automake \
  libtool \
  nasm \
  libjpeg-turbo-utils \
  && \
  pip install --upgrade awscli==1.14.5 s3cmd==2.0.1 python-magic && \
  apk -v --purge del py-pip && \
  rm /var/cache/apk/*
# https://rn4ru.com/blog/posts/pelican-on-docker-for-mac/
# https://qiita.com/5t111111/items/d745af778969bf00f038

FROM alpine:latest

MAINTAINER Ponkotsu <ponkotsu.ni@gmail.com>

RUN echo -e "@edge http://nl.alpinelinux.org/alpine/edge/main\n@testing http://nl.alpinelinux.org/alpine/edge/testing\n@community http://nl.alpinelinux.org/alpine/edge/community" >> /etc/apk/repositories

RUN apk -U add --no-cache \
    python3 \
    perl \
    make \
    bash \
    git \
    openssh \
    && pip3 install --upgrade pip \
    && pip3 install pelican markdown ghp-import

EXPOSE 8000
#WORKDIR /site

FROM alpine:3.15.0

RUN sed -i "s/dl-cdn.alpinelinux.org/mirrors.aliyun.com/g" /etc/apk/repositories \
    && apk update \
    && apk add apache2-utils \
    && rm -rf /var/cache/apk/*

ENTRYPOINT ["htpasswd", "-Bbn"]
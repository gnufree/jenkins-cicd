FROM alpine:3.4

LABEL zhiwenjun "zhiwenjun001@163.com"

ENV LANG C.UTF-8

RUN sed -i 's/http:\/\/dl-cdn.alpinelinux.org/https:\/\/mirrors.aliyun.com/g' /etc/apk/repositories \
    && apk update && apk add --no-cache ca-certificates tzdata bash curl openjdk8 git \
    && rm -rf /var/cache/apk/* \
    && ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && echo "Asia/Shanghai" > /etc/timezone


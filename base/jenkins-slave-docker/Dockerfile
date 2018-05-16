FROM harbor.kanche.com/cicd/jnlp-slave:v1
MAINTAINER  zhiwenjun <wenjun.zhi@kanche.com>

USER root

RUN curl -fSL "https://mirrors.aliyun.com/docker-ce/linux/static/stable/x86_64/docker-18.03.1-ce.tgz" -o docker.tgz \
    && tar -xzvf docker.tgz \
    && mv docker/* /usr/local/bin/ \
    && rmdir docker \
    && rm docker.tgz \
    && chmod +x /usr/local/bin/docker


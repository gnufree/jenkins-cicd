FROM harbor.kanche.com/cicd/docker-slave:v1
MAINTAINER zhiwenjun <zhiwenjun001@163.com>

LABEL Description="This is a base image, which allows connecting Jenkins agents via JNLP protocols" Vendor="Jenkins project" Version="3.19"

COPY jenkins-slave /usr/local/bin/jenkins-slave

ENTRYPOINT ["jenkins-slave"]

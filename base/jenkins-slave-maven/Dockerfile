FROM harbor.kanche.com/cicd/jnlp-slave:v1

MAINTAINER  zhiwenjun <wenjun.zhi@kanche.com>

USER root
ENV MAVEN_HOME /usr/share/maven

RUN curl -fsSl http://mirrors.hust.edu.cn/apache/maven/maven-3/3.3.9/binaries/apache-maven-3.3.9-bin.tar.gz |tar -zxC /usr/share/ \
    && mv /usr/share/apache-maven-3.3.9 /usr/share/maven \
    && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn 


USER jenkins

ENV USER_HOME_DIR /home/jenkins
ENV MAVEN_CONFIG "$USER_HOME_DIR/.m2"
COPY settings.xml ${MAVEN_HOME}/conf/settings.xml




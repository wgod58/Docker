FROM centos:7
MAINTAINER zed

RUN yum install -y wget

RUN cd /

ADD jdk-8u192-linux-x64.tar.gz /
ADD apache-tomcat-8.5.37.tar.gz /

ENV JAVA_HOME=/jdk1.8.0_192
ENV JRE_HOME=/jdk1.8.0_192/jre
ENV PATH=$PATH:/jdk1.8.0_192/bin
CMD ["/apache-tomcat-8.5.37/bin/catalina.sh", "run"]
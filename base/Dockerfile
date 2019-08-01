FROM fedora:latest

MAINTAINER Bruno Panuto <bl.panuto@gmail.com>

ARG version=2.0.0

RUN yum update -y && yum install -y java tar

RUN curl -s http://archive.apache.org/dist/storm/apache-storm-2.0.0/apache-storm-$version.tar.gz | \
      tar zxf - -C /opt && \
      mv /opt/apache-storm-$version /opt/apache-storm

ADD configure.sh /

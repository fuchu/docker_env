FROM ubuntu:14.04.3
MAINTAINER Kevin Zhou <gitofkevin@outlook.com>
ENV REFRESHED_AT 2016-08-31

RUN apt-get update && apt-get install -yqq python-pip
RUN pip install shadowsocks
EXPOSE 8080

ENTRYPOINT ["/usr/local/bin/ssserver"]

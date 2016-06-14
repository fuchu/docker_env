FROM ubuntu
MAINTAINER Kevin Zhou <gitofkevin@outlook.com>
ENV REFRESHED_AT 2016-06-14

RUN apt-get install -yqq software-properties-common
RUN apt-add-repository  ppa:ansible/ansible
RUN apt-get -yqq update
RUN apt-get install -yqq ansible
RUN echo '[local]\nlocalhost\n' > /etc/ansible/hosts
RUN mkdir /home/kevin
RUN useradd -g root kevin
RUN usermod -s /bin/bash -d /home/kevin kevin
RUN chown -R kevin:root /home/kevin
VOLUME [ "/home/kevin" ]
CMD []

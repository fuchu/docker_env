FROM centos:centos7
MAINTAINER Kevin Zhou <gitofkevin@outlook.com>
ENV REFRESHED_AT 2016-06-14

RUN yum clean all && \
    yum -y install epel-release && \
    yum -y install PyYAML python-jinja2 python-httplib2 python-keyczar python-paramiko python-setuptools git python-pip
RUN mkdir /etc/ansible/
RUN echo -e '[local]\nlocalhost\n' > /etc/ansible/hosts
RUN pip install ansible
RUN useradd kevin
RUN mkdir /home/kevin/.ssh
RUN mkdir /home/kevin/server-config
RUN chmod 600 /home/kevin/.ssh
RUN chown -R kevin:kevin /home/kevin
RUN yum -y install vim
VOLUME [ "/home/kevin/.ssh" , "/home/kevin/server-config" ]
CMD []

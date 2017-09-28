FROM centos:latest

MAINTAINER BEN CHAABEN Wissem <benchaaben.wissem@gmail.com>

#Prevent rpm errors
ENV TERM=xterm-265color

#Install Ansible
RUN yum -y update && \
    yum -y install ansible

#Add voulume for ANsible playbooks
VOLUME [ "/ansible" ]
WORKDIR /ansible

#Entrypoint
ENTRYPOINT [ "ansible-playbook" ]
CMD [ "site.yml" ]


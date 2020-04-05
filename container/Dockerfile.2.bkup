# Getting base image
FROM schmots1/netapp-ansible

MAINTAINER ken hillier <ken.hillier@gmail.com>

# Command to run something within image during creation
RUN yum update -y &&\
    yum install -y git

RUN mkdir /git &&\
    cd /git &&\
    git clone https://github.com/wolftales/netapp-ansible-demo.git /git/.

#RUN mkdir /etc/ansible &&\
#    mkdir /etc/ansible/content &&\
#    git clone https://github.com/netapp/ansible.git /etc/ansible/content

#Set working directory
#WORKDIR /git/Ansible-Demo

#Configuring NetApp Ansible roles
#COPY ansible-netapp-roles.cfg /etc/ansible/ansible.cfg

# CMD run something on command line
# #RUN is executed when you create an image
# #CMD is run only when you create a container out of the image, later
#CMD ["echo", "Hello World...! from my first my first docker image"]


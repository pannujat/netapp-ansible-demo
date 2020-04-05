# Getting base image
FROM schmots1/netapp-ansible

MAINTAINER ken hillier <ken.hillier@gmail.com>

# Command to run something within image during creation
RUN yum update -y &&\
    yum install -y git

RUN mkdir /git &&\
    cd /git &&\
    git clone https://github.com/wolftales/netapp-ansible-demo.git /git/.

#Set working directory
#WORKDIR /git/Ansible-Demo



#
# Ansible Dockerfile
#
# https://github.com/ryanfitz/dockerfiles
#

FROM ubuntu:14.04
MAINTAINER Ryan Fitzgerald, ryan.fitz1@gmail.com

RUN DEBIAN_FRONTEND=noninteractive apt-get install -y -q python-software-properties software-properties-common
RUN apt-add-repository ppa:rquillo/ansible
RUN apt-get update
RUN apt-get install -y ansible

# Define default command.
CMD ["/bin/bash"]

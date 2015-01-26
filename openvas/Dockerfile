FROM centos:latest
MAINTAINER sebbrochet <contact@sebbrochet.com>

RUN yum -y install wget && wget -q -O - http://www.atomicorp.com/installers/atomic | sh && yum -y upgrade && yum -y install openvas

RUN wget -q -O - http://downloads.arachni-scanner.com/arachni-1.0.6-0.5.6-linux-x86_64.tar.gz | tar xz -C /root

ENV PATH /root/arachni-1.0.6-0.5.6/bin:$PATH

EXPOSE 9392


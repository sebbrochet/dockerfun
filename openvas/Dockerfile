FROM centos:latest
MAINTAINER sebbrochet <contact@sebbrochet.com>

RUN yum -y install wget && wget -q -O - http://www.atomicorp.com/installers/atomic | sh && yum -y update && yum -y install openvas

EXPOSE 9392


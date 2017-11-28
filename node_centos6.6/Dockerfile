
FROM centos:centos6.6

RUN yum -y update; yum clean all
RUN yum -y install epel-release; yum clean all
RUN curl --silent --location https://rpm.nodesource.com/setup_8.x | bash -
RUN yum -y install nodejs; yum clean all

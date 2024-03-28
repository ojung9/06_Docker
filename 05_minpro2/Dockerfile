FROM centos:7

RUN yum -y install httpd php && yum clean all

ADD src.tar /var/www/html

EXPOSE 80
VOLUME /var/www/html /var/log/httpd

ENTRYPOINT /usr/sbin/httpd -D FOREGROUND
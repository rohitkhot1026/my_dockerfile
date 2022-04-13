FROM centos:7
RUN yum -y install httpd
copy index.html /var/www/html
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
EXPOSE 80




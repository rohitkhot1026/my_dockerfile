FROM centos:7
RUN yum update -y
RUN yum install httpd unzip -y 
ADD https://www.free-css.com/assets/files/free-css-templates/download/page275/edulab.zip /var/www/html
WORKDIR /var/www/html
RUN  unzip edulab.zip
RUN cp -rvf edulab/* .
RUN rm -rf 	.zip 
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]
EXPOSE 80

FROM ubuntu:latest
#LABEL "Author"="ganesh"
#LABEL "Project"="nano"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install unzip
RUN apt install apache2 -y
#CMD ["/usr/sbin/apache2ctl","-D", "FORGROUND"]
#EXPOSE 80
WORKDIR /var/www/html
RUN rm -f index.html
VOLUME /var/log/apache2
ADD  https://www.free-css.com/assets/files/free-css-templates/download/page275/edulab.zip /var/www/html
RUN unzip edulab.zip
RUN cp -R edulab/* .
CMD ["/usr/sbin/apache2ctl","-D", "FORGROUND"]
EXPOSE 80

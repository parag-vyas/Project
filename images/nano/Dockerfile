FROM ubuntu:latest
LABEL Auther="Parag"
ENV DEBIAN_FRONTEND=noninteractive
RUN  apt update && install git -y
RUN apt install apache2 
CMD ["/usr/sbin,apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
WORKDIR /var/www/htmp    (if we run any command from docker exec this will run from this directory)
VOLUME  /var/log/apache2
ADD nano.tar.gz /var/www/html    (untar contain in /var/www.html)
#COPY nano.tar.gz /var/www/html    (only take and dump into directory)

FROM ubuntu:16.04
 
RUN apt update -y 
RUN apt install apache2 php libapache2-mod-php php-mysql -y
 
COPY apache-conf /etc/apache2/apache2.conf
COPY dir.conf /etc/apache2/mods-enabled
COPY index.php /var/www/html
 
EXPOSE 80

ENV WEB_MSG Docker container Website welcomes!
ENV WEB_MSG_2 Additional info here..

CMD ["/usr/sbin/apache2ctl", "-DFOREGROUND"]

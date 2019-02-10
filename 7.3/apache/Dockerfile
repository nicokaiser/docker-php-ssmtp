FROM php:7.3-apache
LABEL maintainer "Nico Kaiser <nico@kaiser.me>"

RUN apt-get update && \
    apt-get install -y ssmtp && \
    apt-get clean && \
    echo 'sendmail_path = "/usr/sbin/ssmtp -t"' > /usr/local/etc/php/conf.d/mail.ini

FROM php:7.4-apache

# install the ssl-cert package which will create a "snakeoil" keypair
# RUN apt-get update \
#  && DEBIAN_FRONTEND=noninteractive apt-get install -y ssl-cert \
#  && rm -r /var/lib/apt/lists/*

# enable ssl module and enable the default-ssl site
RUN a2enmod rewrite
# RUN a2ensite default-ssl
RUN a2enmod ssl

COPY ./php.ini /usr/local/etc/php/

EXPOSE 80
EXPOSE 443
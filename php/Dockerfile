FROM php:7.1-apache  

RUN apt-get update
RUN docker-php-ext-install mysqli
RUN apt-get install -y libcurl4-openssl-dev pkg-config libssl-dev
RUN pecl install mongodb-1.10.0 -y \
    && docker-php-ext-enable mongodb



#RUN apt-get update \
#    && apt-get install -y default-mysql-client

#RUN cp /etc/apache2/mods-available/rewrite.load /etc/apache2/mods-enabled/ && \
#    cp /etc/apache2/mods-available/headers.load /etc/apache2/mods-enabled/

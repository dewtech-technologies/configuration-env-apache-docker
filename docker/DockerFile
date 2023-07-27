FROM php:8.2-apache

RUN apt-get update && apt-get install -y \
    git   \
    curl  \
    zip \
    unzip \
    libapache2-mod-php

RUN a2enmod rewrite

WORKDIR /var/www/html

COPY . /var/www/html

EXPOSE 80

CMD ["apache2-foreground"]

FROM php:5.6-apache
COPY config/php.ini /usr/local/etc/php/
RUN  apt-get update && apt-get install -y libpng12-dev && docker-php-ext-install -j$(nproc) gd mysqli

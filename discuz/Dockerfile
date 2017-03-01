FROM php:7.0-apache
RUN  apt-get update && apt-get install -y curl libcurl4-gnutls-dev libpng12-dev && docker-php-ext-install -j$(nproc) curl gd pdo pdo_mysql mbstring mysqli

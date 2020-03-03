FROM php:7.2.3-fpm

RUN pecl install xdebug && \
    docker-php-ext-enable xdebug

RUN apt-get update && apt-get install -y mysql-client

RUN docker-php-ext-install pdo_mysql
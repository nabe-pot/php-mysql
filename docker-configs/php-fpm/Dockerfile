FROM php:7.2.3-fpm

RUN apt-get update && apt-get install -y \
mysql-client \
libjpeg62-turbo-dev \
libpng-dev

RUN pecl install xdebug gd && \
    docker-php-ext-enable xdebug && \
    docker-php-ext-configure gd --with-jpeg-dir=/usr && \
    docker-php-ext-install -j$(nproc) gd

RUN docker-php-ext-install pdo_mysql
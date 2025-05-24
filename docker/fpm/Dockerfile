FROM php:8.2-fpm-alpine

WORKDIR /var/www/site

COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer

RUN docker-php-ext-install mysqli

RUN docker-php-ext-install pdo pdo_mysql

RUN docker-php-ext-enable mysqli
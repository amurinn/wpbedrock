FROM php:8.2.0-fpm

# Install PHP extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql && docker-php-ext-enable mysqli

RUN apk add --no-cache shadow
RUN deluser xfs
RUN usermod -u 1000 www-data
RUN groupmod -g 33 www-data

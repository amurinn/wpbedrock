FROM php:8.2.0-fpm-alpine

# Install Bash
RUN apk add --no-cache bash

# Install PHP extensions
RUN docker-php-ext-install mysqli pdo pdo_mysql && docker-php-ext-enable mysqli

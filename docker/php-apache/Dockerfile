ARG PHP_VERSION

FROM php:${PHP_VERSION}-apache

ARG USER_ID
ARG GROUP_ID

RUN apt-get update
RUN docker-php-ext-install pdo pdo_mysql

RUN usermod -u ${USER_ID} www-data && \
    groupmod -g ${GROUP_ID} www-data

RUN a2enmod rewrite headers

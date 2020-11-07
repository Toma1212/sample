FROM php:7.2-fpm
COPY php.ini /usr/local/etc/php/

RUN apt-get update \
    &&  curl -sL https://deb.nodesource.com/setup_12.x | bash - \
    && apt-get install -y nodejs \
    && npm install npm@latest -g \
    && apt-get install -y zlib1g-dev mariadb-client \
    && docker-php-ext-install zip pdo_mysql

COPY --from=composer /usr/bin/composer /usr/bin/composer

ENV COMPOSER_ALLOW_SUPERUSER 1

ENV COMPOSER_HOME /composer

ENV PATH $PATH:/composer/vendor/bin


WORKDIR /var/www/html

RUN composer global require "laravel/installer"
FROM php:7.4.11-fpm-buster

RUN apt-get update && apt-get install vim -y && \
    apt-get install openssl -y && \
    apt-get install libssl-dev -y && \
    apt-get install wget -y && \
    apt-get install git -y

RUN docker-php-ext-install pdo_mysql

RUN apt-get autoremove -y && rm -rf /var/lib/apt/lists/*

CMD php-fpm
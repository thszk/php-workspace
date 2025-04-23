FROM php:8.3.20-apache

ARG USERNAME
ARG USERID

RUN groupadd -g ${USERID} ${USERNAME} && \
    useradd -m -u ${USERID} -g ${USERNAME} ${USERNAME} && \
    docker-php-ext-install \
    pdo \
    pdo_mysql

USER ${USERNAME}
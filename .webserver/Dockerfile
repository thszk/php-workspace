FROM php:8.3.20-apache

ARG USERNAME
ARG USERID

RUN groupadd -g ${USERID} ${USERNAME} && \
    useradd -m -u ${USERID} -g ${USERNAME} ${USERNAME} && \
    apt update && \
    apt install -y \
        libxml2-dev && \
    docker-php-ext-install \
        pdo \
        pdo_mysql \
        xml

USER ${USERNAME}
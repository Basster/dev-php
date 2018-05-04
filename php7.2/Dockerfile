FROM debian:stretch-slim

MAINTAINER Ole Rößner <o.roessner@neusta.de>

RUN apt-get update && apt-get install -y --no-install-recommends \
    wget \
    lsb-release \
    apt-transport-https \
    ca-certificates

RUN wget -O /etc/apt/trusted.gpg.d/php.gpg https://packages.sury.org/php/apt.gpg \
    && sh -c 'echo "deb https://packages.sury.org/php/ $(lsb_release -sc) main" > /etc/apt/sources.list.d/php.list'

RUN apt-get update && apt-get install -y --no-install-recommends \
  php7.2-apcu \
  php7.2-common \
  php7.2-readline \
  php7.2-fpm \
  php7.2-cli \
  php7.2-mysql \
  php7.2-curl \
  php7.2-intl \
  php7.2-mbstring \
  php7.2-opcache \
  php7.2-json \
  php7.2-pdo \
  php7.2-memcached \
  php7.2-zip \
  php7.2-xsl \
  php7.2-gmagick \
  php7.2-xdebug

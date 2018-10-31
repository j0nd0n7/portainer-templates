FROM wordpress

COPY ./uploads.ini /usr/local/etc/php/conf.d/uploads.ini

RUN apt-get update \
    && apt-get install -y zlib1g-dev \
    && rm -rf /var/lib/apt/lists/* \
    && docker-php-ext-install zip
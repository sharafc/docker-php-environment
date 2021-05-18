FROM php:7.4-cli-alpine
RUN apk add --no-cache --virtual .build-deps $PHPIZE_DEPS \
    && pecl install xdebug-3.0.4 \
    && docker-php-ext-enable xdebug \
    && apk del -f .build-deps
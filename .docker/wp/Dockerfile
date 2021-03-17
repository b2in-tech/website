FROM wordpress:5.7.0-fpm-alpine

RUN apk add --no-cache shadow

RUN usermod -u 1000 www-data
RUN chown -R www-data:www-data /var/www/html
USER www-data

CMD ["php-fpm"]
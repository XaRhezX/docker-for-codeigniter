FROM php:7.2-fpm
WORKDIR /var/www/html/
RUN docker-php-ext-install mysqli
RUN usermod -u 1000 www-data && groupmod -g 1000 www-data;
ADD . /var/www/html/
RUN chown -R www-data:www-data /var/www/html/
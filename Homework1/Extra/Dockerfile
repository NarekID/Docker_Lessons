FROM debian:latest
RUN apt update -y && apt install -y nginx php7.3-fpm:
COPY nginx_default /etc/nginx/sites-available/default
COPY php.ini /etc/php/7.3/fpm/php.ini
COPY phpinfo.php /var/www/html/phpinfo.php
EXPOSE 80
ENTRYPOINT service php7.3-fpm start && nginx -g 'daemon off;'

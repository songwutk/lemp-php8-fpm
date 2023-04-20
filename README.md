# Generate Self signed Certificate

sudo openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout custom.key -out custom.crt


# Add new php8 extension


docker exec -it php8-fpm /bin/sh

apk add php8-(new extension)

vim /usr/local/etc/php/conf.d/docker-php-ext-sodium.ini 


cp /usr/local/etc/php/php.ini-production /usr/local/etc/php/php.ini
vim /usr/local/etc/php/php.ini

php -m to review installed extension

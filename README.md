# docker-ubuntu16-lamp-xdebug-ssl-phpunit
Basic ubuntu16 installation along with apache, mysql and PHP7 Added modules are Xdebug-SSL-PHPUnit-rabbitMQ server

# Ubuntu 16 Server with PHP 7 - Apache - Mysql

[![](https://images.microbadger.com/badges/image/shinigamigood/docker-ubuntu16-lamp-xdebug-ssl-phpunit.svg)](https://microbadger.com/images/shinigamigood/docker-ubuntu16-lamp-xdebug-ssl-phpunit "Get your own image badge on microbadger.com") [![](https://images.microbadger.com/badges/version/shinigamigood/docker-ubuntu16-lamp-xdebug-ssl-phpunit.svg)](https://microbadger.com/images/shinigamigood/docker-ubuntu16-lamp-xdebug-ssl-phpunit "Get your own version badge on microbadger.com")

This creates a Docker container running PHP, Apache, and Mysql on ubuntu 16

## Why another container?  

I just wanted all the PHP libraries I tend to use.

 I also wanted to create frequently needed modules needed by developers including Xdebug, phpUnit, SSL certificate generation and access, etc.

The installed Mysql server has no password in it.

## Run Example

- `docker run -d -p 80:80 -p 443:443 -v devInt:/var/www/html  --name=DeveloperInterface shinigamigood/ubuntu16-lamp-xdebug-ssl-phpunit`


## Docker Environment Variables

- `PHP_BEFORE`: command(s) to run prior to running `composer install` 
- `PHP_COMPOSER_FLAGS`: flags to include with `composer install` (ex: --prefer-dist --no-dev)
- `PHP_AFTER`: command(s) to run after `composer install`

##  Extensions:

- Xdebug
- SSL + config
- phpUnit
- a2enmod
- Rabbit MQ server
- Git

## PHP-7 Extensions:

- libapache2
- libzend
- curl
- imagick
- mbstring
- mcrypt
- memcached
- ... and a bunch of others.  Read the Dockerfile.


test

Configuration
- PHP
- Composer
- Nginx
- Mysql
- phpMyAdmin

RUN Docker-compose
1. make image image from dockerfile or download image "docker pull herdanis/php7.3-composer-laravel:1.0"
2. change docker-compose.dev.yml => docker-compose.yml
3. change port in docker-compose.yml to unused port (ex = 82:80)
4. copy or change nginx dev configuration
 - /nginx/default.dev.conf => /nginx/default.conf
5. copy or change php.ini configuration
 - /php/php.dev.ini => /php/php.ini
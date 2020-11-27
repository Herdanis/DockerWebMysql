Configuration
- PHP
- Composer
- Nginx
- Mysql
- phpMyAdmin

RUN Docker-compose
1. change docker-compose.dev.yml => docker-compose.yml
2. change port in docker-compose.yml to unused port (ex = 82:80)
3. copy or change nginx dev configuration
 - /nginx/default.dev.conf => /nginx/default.conf
4. copy or change php.ini configuration
 - /php/php.dev.ini => /php/php.ini
5. run docker-compose it will create mysql and app folder
6. copy and paste or clone project from github
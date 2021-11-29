# About Test

## Tech
- Laravel 7
- Php 7.4
- Mysql 5.5

## Setup
- docker-compose -f docker/docker-compose.yml up --build
- docker-compose -f docker/docker-compose.yml exec app composer install
- docker-compose -f docker/docker-compose.yml exec app cp .env.example .env
- docker-compose -f docker/docker-compose.yml exec app php artisan key:generate
- docker-compose -f docker/docker-compose.yml exec app php artisan cache:clear
- docker-compose -f docker/docker-compose.yml exec app php artisan config:clear

# Docker for basic php projects

## Build the image

```` bash
docker build -t lwa/php-basic . 
````

## Start container

```` bash
docker run -d -p 80:80 --name my-php-app lwa/php-basic
````

## Start container with volumes

```` bash
docker run -d -p 80:80 --name my-php-app -v /home/roberth/Desktop/docker-basic-php/src:/var/www/html lwa/php-basic
````

## Stop container

```` bash
docker stop my-php-app
````

### DOCS

- [php docker image](https://hub.docker.com/_/php)
- [YouTube tutorial](https://youtu.be/vuep0XWZNY8)

### Some commands

1. Start php local server

```` bash
cd ./src
php -S localhost:8000
````
### Regards

Roberth Rodriguez,
[Laravel the web artisan](https://www.facebook.com/laravelthewebartisan).

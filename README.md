# php-production-cli
Docker Container for running PHP cli commands in production


## Features

* Ubuntu Linux 
* PHP 7.1 cli
* Commonly used PHP extensions (php7.1-curl, php7.1-json, php7.1-mbstring, php7.1-mcrypt, php7.1-mysql etc)
* Git
* Curl
* vi
* Composer
* MySQL and PostgreSQL client

### Usage


use it as a base image for your container
```
FROM buonzz/php-production-cli:latest
```

or, login to it and invoke PHP commands

```
docker exec -ti  php-production-cli bash
```


## Building the image

```
./build.sh
```

## Running the image

```
docker run php-production-cli
```
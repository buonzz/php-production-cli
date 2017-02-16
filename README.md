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

or use it directly as an interactive shell
```
docker run -it buonzz/php-production-cli:0.0.1 /bin/bash
```

## Building the image

You'll only need to re-build the docker image if you want to install any additional software. After you had tweaked the Dockerfile. just run the command below to re-build it.

```
./build.sh
```

## Running the image

```
docker run php-production-cli
```
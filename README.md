# Alpine PHP


[![Build Status](https://travis-ci.org/luzeduardo/alpine-php-fpm.svg?branch=master)](https://travis-ci.org/luzeduardo/alpine-php-fpm)

## Getting The Image

This image is published in the [Docker Hub](https://hub.docker.com/r/luzeduardo/alpine-php-fpm/).

Alternatively you can clone this repository and build the image using the `docker build` command.

```Shell
docker build -t repository/imagename:tag .
```

### PHP Configuration

The config is set using environments listed below on build.

```Ini
ENV TIMEZONE            America/Sao_Paulo
ENV PHP_MEMORY_LIMIT    512M
ENV MAX_UPLOAD          100M
ENV PHP_MAX_FILE_UPLOAD 200
ENV PHP_MAX_POST        100M
```

Change it in `Dockerfile` and you can rebuild your image.


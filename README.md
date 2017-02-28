# docker-php7-fpm-stack
This Docker image (based on php7-fpm) is intended to run php7 code which may need to use Mysqli or GD libraries.

## Installation:
### Build image
```sh
$ docker build -t "cdue/docker-php7-fpm-stack:latest" .
```

### Or get it from the Docker Hub
```sh
$ docker pull "cdue/docker-php7-fpm-stack"
```

## Run a bash with a volume mounted:
```sh
$ docker run --rm -it -v $(pwd):/app/ "cdue/docker-php7-fpm-stack:latest" /bin/bash
```
Windows users must add a / before $(pwd)

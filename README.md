![latest 10](https://img.shields.io/badge/latest-12-green.svg?style=flat)
![node 10](https://img.shields.io/badge/node-12-brightgreen.svg) ![License MIT](https://img.shields.io/badge/license-MIT-blue.svg) [![Build Status](https://travis-ci.org/Pipekung/docker-node-oracle.svg?branch=master)](https://travis-ci.org/Pipekung/docker-node-oracle) [![](https://img.shields.io/docker/stars/pipekung/node-oracle.svg)](https://hub.docker.com/r/pipekung/node-oracle 'DockerHub') [![](https://img.shields.io/docker/pulls/pipekung/node-oracle.svg)](https://hub.docker.com/r/pipekung/node-oracle 'DockerHub')

# Supported tags

- [```12```, ```node12-oci19```, ```latest```](https://github.com/Pipekung/docker-node-oracle/blob/master/Dockerfile)
- [```10```, ```node10-oci19```](https://github.com/Pipekung/docker-node-oracle/blob/master/mainline/node10-oci19/Dockerfile)

# How to use this image

## Using docker run

```console
$ docker run -it --rm -p 9000:9000 -e NODE_ENV=production -v /path/to/your/project:/usr/src/app pipekung/node-oracle node app.js
```

## Using docker-compose

``` yml
version: "2"
services:
  app:
    image: pipekung/node-oracle
    environment:
      - NODE_ENV=production
    volumes:
      - /path/to/your/project:/usr/src/app
    ports:
      - 9000:9000
    command: node app.js
```

Run docker-compose:

```console
$ docker-compose up -d
```

# Reference

- [node official](https://hub.docker.com/_/node)

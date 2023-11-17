# Docker Image für PHP_Depend

[PHP Depend](https://github.com/pdepend/pdepend) is a static analysis tool for PHP, 
mainly for seeing flaws in your code because you have to many dependencies in a class etc.

This repository provides a Docker image for PHP depend.

[![fabiang/pdepend](https://img.shields.io/docker/pulls/fabiang/pdepend.svg)](https://hub.docker.com/r/fabiang/pdepend)
[![fabiang/pdepend](https://badgen.net/github/license/fabiang/docker-pdepend)](https://github.com/fabiang/docker-pdepend)
[![Docker Image](https://github.com/fabiang/docker-pdepend/actions/workflows/docker.yml/badge.svg)](https://github.com/fabiang/docker-pdepend/actions/workflows/docker.yml)

## Available tags

* 2.15.1, 2.15.1-alpine, 2.15, 2.15-alpine, 2, 2-alpine, latest, latest-alpine

## Usage

```bash
docker run --rm -it fabiang/pdepend:2-alpine --help
```

## License

All other parts of the library are licensed under [BSD 2-Clause License](LICENSE.md).

# Docker Image for PHP_Depend

[PHP Depend](https://github.com/pdepend/pdepend) is a static analysis tool for PHP, 
mainly for seeing flaws in your code because you have to many dependencies in a class etc.

This repository provides a Docker image for PHP depend.

[![fabiang/pdepend](https://img.shields.io/docker/pulls/fabiang/pdepend.svg)](https://hub.docker.com/r/fabiang/pdepend)
[![fabiang/pdepend](https://badgen.net/github/license/fabiang/docker-pdepend)](https://github.com/fabiang/docker-pdepend)
[![Docker Image](https://github.com/fabiang/docker-pdepend/actions/workflows/docker.yml/badge.svg)](https://github.com/fabiang/docker-pdepend/actions/workflows/docker.yml)

## Available tags

[See Docker Hub page](https://hub.docker.com/r/fabiang/pdepend/tags?page=1&ordering=name)

## Usage

```bash
docker run --rm -it fabiang/pdepend:2-alpine --help
```

## License

PHP Depend is licensed under BSD 3-Clause License. This software is licensed under [BSD 2-Clause License](LICENSE.md).

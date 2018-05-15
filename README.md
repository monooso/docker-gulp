# Gulp for Docker #
Ephemeral Docker container for installing Node modules, and running Gulp commands (such as `gulp watch`).

## Typical usage ##

```
$ docker run --rm -v /path/to/app:/home/node/app monooso/docker-gulp:node8 npm install --verbose
$ docker run --rm -v /path/to/app:/home/node/app monooso/docker-gulp:node8 gulp --tasks
```

# Laravenv

[![DockerHub Pulls](https://img.shields.io/docker/pulls/niccolomeloni/laravenv.svg)](https://hub.docker.com/r/niccolomeloni/docker-nativescript-cli/) [![DockerHub Stars](https://img.shields.io/docker/stars/niccolomeloni/laravenv.svg)](https://hub.docker.com/r/niccolomeloni/docker-nativescript-cli/) [![GitHub Stars](https://img.shields.io/github/stars/niccolomeloni/laravenv.svg?label=github%20stars)](https://github.com/niccolomeloni/laravenv) [![GitHub License](https://img.shields.io/github/license/niccolomeloni/laravenv.svg)](https://github.com/niccolomeloni/docker-nativescript-cli)

Laravenv is a [docker](https://www.docker.com/) image ready to put running [Laraver](https://laravel.com/) framework. Take a look around and feel free to suggest improvements.

# Supported tags and respective `Dockerfile` links

-	[`7.3-slim`, `slim` (*slim/7.3/Dockerfile*)](https://github.com/niccolomeloni/laravenv/blob/master/7.3/slim/Dockerfile)

## Laravel Server Requirements

| Dependencies |
| ------------ |
| PHP >= 7.1.3 |
| OpenSSL PHP Extension |
| PDO PHP Extension |
| Mbstring PHP Extension |
| Tokenizer PHP Extension |
| XML PHP Extension |
| Ctype PHP Extension |
| JSON PHP Extension |
| BCMath PHP Extension |

More [here](https://laravel.com/docs/5.8#server-requirements)

## Getting Started

All the image tags comes with following features out of the box:
 * [Xdebug](https://xdebug.org/docs/remote)
 * [Composer](https://getcomposer.org/)
 * [hirak/prestissimo](https://github.com/hirak/prestissimo)
 * [laravel/installar](https://github.com/laravel/installer)

### The `slim` tag 

In order to get started type following command from root directory of your Laravel project

```sh
docker run --rm -it -p 8000:8000 -v $PWD:/laravel niccolomeloni/laravenv:slim php artisan serve --host 0.0.0.0
```

## License
This project is licensed under the MIT license by Niccolò Meloni.
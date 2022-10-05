
# Symfony 6 + PHP 8.1 with Docker

**ONLY for DEV, not for production**

A very simple Docker-compose to discover Symfony 6 with PHP 8.1 in 5 minutes
## Run Locally

Clone the project

```bash
  git remote add origin git@github.com:amin2015/CVGenerator.git
```

Run the docker-compose

```bash
  docker-compose build
  docker-compose up -d
```

Create Host

```bash
 php -S localhost:8080 -t public
```

*Your application is available at http://localhost:8080*

If you need a database, modify the .env file like this example:

```yaml
  DATABASE_URL="postgresql://symfony:ChangeMe@database:5432/app?serverVersion=13&charset=utf8"
```

## Ready to use with

This docker-compose provides you :

- PHP-8.0.13-cli (Debian)
    - Composer
    - Symfony CLI
    - and some other php extentions
    - nodejs, npm, yarn
- postgres:13-alpine
- mailcatcher


## Requirements

Out of the box, this docker-compose is designed for a Linux operating system, provide adaptations for a Mac or Windows environment.

- Linux (Ubuntu 20.04 or other)
- Docker
- Docker-compose

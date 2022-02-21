# Laravel

The PHP Framework for Web Artisans.  
<https://laravel.com/>  
Dcocumentation is [here](https://readouble.com/laravel/).

## Environment

Using Docker to build an environment called the ***LEMP*** environment.  

| Middleware | Initial | Middleware name |
| :---: | :---: | :---: |
| Operating System | L | Linux |
| Web server | E | Nginx |
| DB server | M | MySQL |
| Application | P | PHP(F: Laravel) |

## Notice

Using git to manage it, be sure to specify the .env file in .gitignore.

## Getting Started

Requirement:

- [Docker](https://www.docker.com/)

## build for image

```
docker compose build
```

## Start for image

```
docker compose up -d
```

## Enter the container using bash

```
docker compose exec app bash
```

If the directory changes to /var/www/html as shown below,  
you are now in the app container.

```
root@51030054f131:/var/www/html#
```

Each string after @ is different.

## Create Laravel projects

- Check to be installed "composer"

```
composer
```

If the following message appears, you have succeeded

```
   ______
  / ____/___  ____ ___  ____  ____  ________  _____
 / /   / __ \/ __ `__ \/ __ \/ __ \/ ___/ _ \/ ___/
/ /___/ /_/ / / / / / / /_/ / /_/ (__  )  __/ /
\____/\____/_/ /_/ /_/ .___/\____/____/\___/_/
                    /_/
Composer version 2.2.6 2022-02-04 17:00:38
```

- Install Laravel

```
composer create-project --prefer-dist laravel/laravel .
```
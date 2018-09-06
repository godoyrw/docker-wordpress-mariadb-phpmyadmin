# Docker YML File 3.3
Docker YML for Wordpress, MariaDB and phpMyAdmin.

[<img src="https://godahtech.com.br/wp-content/uploads/godahtech.com.br_godahtech_logo_h334x148-200x89.png" style="width:140px;"/>](https://godahtech.com.br/)


# Using Technology

![Docker](./assets/github-dwmp.png)


## Usage with docker-compose and arbitrary server

This will run phpMyAdmin with arbitrary server - allowing you to specify MySQL/MariaDB
server on login page.

Using the docker-compose.yml from https://github.com/phpmyadmin/docker

```
docker-compose up -d
```


## Environment MariaDB variables summary

* ``MYSQL_ROOT_PASSWORD`` - define root password of the MySQL server.
* ``MYSQL_DATABASE`` - define database name of the MySQL server.
* ``MYSQL_USER`` - define user name of the MySQL server.
* ``MYSQL_PASSWORD`` - define user password of the MySQL server.


## Environment Wordpress variables summary

* ``VIRTUAL_HOST`` - define virtual host of the Wordpress website.
* ``VIRTUAL_PORT`` - define virtual port of the Wordpress website.
* ``WORDPRESS_DB_HOST`` - define Mysql address/host of the Wordpress website.
* ``WORDPRESS_DB_NAME`` - define database name of the Wordpress website.
* ``WORDPRESS_TABLE_PREFIX`` - define database prefix of the Wordpress website.
* ``WORDPRESS_DB_PASSWORD`` - define database password of the Wordpress website.


## Environment phpMyAdmin variables summary

* ``PMA_ARBITRARY`` - when set to 1 connection to the arbitrary server will be allowed
* ``PMA_HOST`` - define address/host name of the MySQL server

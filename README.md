```
       :  Solr     : ~.  
        \         / .   ` ~   
        ,''.___.''.   `.    
          /  !  \  `.    `.    
        '    ;   :    \     `.
                  `       

                                  ______        
                                 \\----\\      __ _  _  _ | /               
                                  \\    \\    (_ |_)|_||_)|/  ______                          ____        
                                   \\    \\   __)|  | || \|\  \\   \\                       /    /
                                 ▒▒ \\____\\___________________\\---\\                     /     |
                             ▒▒  ▒▒  '-----\\-------------------\\----'                    \     \
                             ▒▒  ▒▒  ▒▒  ▒▒ \\___________________\\   ▒▒                   /     \__
                          .__▒▒__▒▒__▒▒__▒▒__\_____________________\__▒▒__▒▒              /          \
                         /                     \   \   \   \   \   \   \   \____________/    /\______\
                        |                                                                   /
  .. -- ~~. ~~ ~ - . ~  |~ . ~ , ~ .  ~ . ~ ~ .  ~ . ~ , ~ .  . .~ . ~ ~ . ~~ . ~...  ~~ / ~.~ ~ -- ~ . ~
                        |                __                                             /
                        |_________      (0 )                                           /
                        | ______   \                                               ___/
                         | ______   |                                             /
                          | ________|                                            /
                           | ______  \                                          /
                            \________ \________________________________________/
```
> Docker container for Laravel Spark

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/websemantics/spark-docker/master/LICENSE) [![GitHub forks](https://img.shields.io/github/forks/websemantics/spark-docker.svg)](https://github.com/websemantics/spark-docker/network) [![GitHub stars](https://img.shields.io/github/stars/websemantics/spark-docker.svg)](https://github.com/websemantics/spark-docker/stargazers)
[![Average time to resolve an issue](http://isitmaintained.com/badge/resolution/websemantics/spark-docker.svg)](http://isitmaintained.com/project/websemantics/spark-docker "Average time to resolve an issue")
[![Percentage of issues still open](http://isitmaintained.com/badge/open/websemantics/spark-docker.svg)](http://isitmaintained.com/project/websemantics/spark-docker "Percentage of issues still open")

## Installation

- Installing docker, https://docs.docker.com/engine/installation/

- Install Spark-Docker container

```
docker pull websemantics/spark-docker
```

- Or clone this repo and run,

```
docker-compose up
```

## Includes

- Nginx 1.8.1
- PHP 7.0
- SQLite
- MySQL 5.7
- Redis
- NodeJS
- Solr
- Blackfire
- Bower
- Gulp
- Composer
- Laravel Envoy
- Laravel Installer
- Spark Installer


## Environment Variables

| Tables        | Are           |
| ------------- |:-------------:|
| APP_NAME      | app |
| APP_DOMAIN      |   spark.dev    |
| APP_EMAIL | spark@websemantics.ca      |
| DB_DATABASE      | spark |
| DB_USERNAME      | spark      |
| DB_PASSWORD | secret      |


## Ports

| Port        | Description           |
| ------------- |:-------------:|
| 80	| Port 80 is open to allow standard HTTP traffic.|
| 443	| Port 443 is open to allow standard HTTPS traffic.|
| 3306	| Port 3306 is open to allow MySQL traffic.|
| 6379	| Port 6379 is open to allow Redis traffic.|
| 8983	| Port 8983 is open to allow Solr traffic.|


## Volumes

| Volume        | Description           |
| ------------- |:-------------:|
| `/var/www/html/app`	| This is the volume that stores your application.|
| `/var/cache/nginx`	| The volume to access Nginx cache.|
| `/var/log/nginx`	| Nginx logs stored in this volume |
| `/var/log/supervisor`	| The volume to access supervisord logs.|
| `/var/lib/mysql`	| Access to mysql from this volume.|
| `/var/lib/solr`	| Access to Solr from this volume.|


## Credits

- This Docker layout is based on https://github.com/laraedit/laraedit-docker.
- Work to install Solar was based on  https://github.com/twinbit/docker-drupal-solr.
- Files in `solr` folder are from https://github.com/composer/packagist

```
   _____                  __      ____             __            
  / ___/____  ____ ______/ /__   / __ \____  _____/ /_____  _____
  \__ \/ __ \/ __ `/ ___/ //_/  / / / / __ \/ ___/ //_/ _ \/ ___/
 ___/ / /_/ / /_/ / /  / ,<    / /_/ / /_/ / /__/ ,< /  __/ /    
/____/ .___/\__,_/_/  /_/|_|  /_____/\____/\___/_/|_|\___/_/     
    /_/ Spark it up ...                                                          

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

## Includes

- Nginx 1.8.1
- PHP 7.0
- SQLite
- MySQL 5.7
- Redis
- NodeJS
- Blackfire
- Bower
- Gulp
- Composer
- Laravel Envoy
- Laravel Installer


## Environment Variables

| Tables        | Are           |
| ------------- |:-------------:|
| APP_NAME      | The default value is app but you can pass whatever you'd like the name of your application to be. setting this parameter will take care of the nginx server block, it will create a database as well as any other configuration necessary to run your application. If you set this variable, make sure to use your new value in place of app any where you come across it in the instructions! |
| APP_DOMAIN      |       |
| APP_EMAIL |       |
| DB_DATABASE      | spark |
| DB_USERNAME      | root      |
| DB_PASSWORD | secret      |


## Ports

| Port        | Description           |
| ------------- |:-------------:|
| 80	| Port 80 is open to allow standard HTTP traffic.|
| 443	| Port 443 is open to allow standard HTTPS traffic.|
| 3306	| Port 3306 is open to allow MySQL traffic.|
| 6379	| Port 6379 is open to allow Redis traffic.|


## Volumes

| Volume        | Description           |
| ------------- |:-------------:|
| `/var/www/html/app`	| This is the volume that stores your application. If you set your APP_NAME environment variable when starting this container, you will need to use your custom value in place of app in this volume. Example - If your `APP_NAME` is set to acme, your volume will be `/var/www/html/acme`.|
| `/var/cache/nginx`	| If you need access to the Nginx cache, this is the volume you are looking for.|
| `/var/log/nginx`	| Nginx acting up? You can check the logs by hooking into this volume |
| `/var/log/supervisor`	| If your application is still not working like it should and your sure you didn't leave out a semi-colon at some point, then you can always check out the supervisord logs. It may also be a good idea to send us anything you find here so we can update the container (if necessary).|

## Credits

This Docker layout is based on https://github.com/laraedit/laraedit-docker

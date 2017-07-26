# php

## laravel + apache + php 環境
```
$ docker build -t laravel laravel/
$ docker run --name laravel --link mysql:mysql -d -p 8081:80 -v `pwd`/application:/tmp/app laravel
```

## mysql docker 環境
```
$ docker build -t mysql mysql/
$ docker run --name mysql -d -e MYSQL_DATABASE=laraveldb -e MYSQL_USER=laravel -e MYSQL_PASSWORD=laravel  -e MYSQL_ROOT_PASSWORD=root mysql
```

# php
## mysql docker 環境
```
$ docker build -t mysql mysql/
$ docker run -d -e MYSQL_DATABASE=laraveldb -e MYSQL_USER=laravel -e MYSQL_PASSWORD=laravel  -e MYSQL_ROOT_PASSWORD=root mysql
```

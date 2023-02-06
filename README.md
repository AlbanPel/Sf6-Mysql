# Sf6-Mysql
##Version:
###Symfony 6 - cli
###Git 2.30.2
###Npm 7.5.2
###Node 12.22.5
###Composer 2.3.7
###PHP 8
###Mysql 8.0

##Run localhost
##First step :Docker
```bash
  docker-compose build
  docker-compose up
```
##Second Step: Connect to the php container
```bash
  docker exec -it php8 bash
  //If line 15-16 are disabled in dockerfile, install cli : wget https://get.symfony.com/cli/installer -O - | bash 
```
##Third step : Create your symfony app
```bash
  symfony new my-project --full
  cd my-project
  symfony serve -d
```
##Four step: add user for write rules
```bash
  adduser username
  chown username:username -R my-project/
```

your app is available on localhost:9000 or http://127.0.0.1:9000





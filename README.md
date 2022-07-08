### Criando arquivo de configuração
```
$ npm init -y
```
### Instalando framework para ajudar no desenvolvimento rapido, minimalista e nao opinativo da api
```
$ npm install express 
```
### Instalando biblioteca para converter dados
```
$ npm install body-parser
```
### Instalando biblioteca que atualiza automaticamente o servidor
```
$ npm install --save-dev nodemon
```
### Instalando banco
```
$ npm install mysql2
```
### Instalando orm e cli
```
$ npm install sequelize sequelize-cli path
```
### Estruturando arquivos iniciais
```
$ npx sequelize-cli init
```
### Rodar programa
```
$ npm run start
```
### Criando volume 
```
docker volume create mysqldata
```
### Rodando imagem
```
docker run -p 3306:3306 -e MYSQL_ALLOW_EMPTY_PASSWORD=true mysql:latest
```
### Acessando imagem
```
mysql -h 127.0.0.1 -P 3306 -u root
```
### Mostrando bancos
```
show databases;
```
### Criando banco
```
create database escola_ingles;
```
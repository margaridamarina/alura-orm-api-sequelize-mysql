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
### Rodando imagem
```
docker-compose up
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
### Criando tabela Pessoas
```
npx sequelize-cli model:create --name Pessoas --attributes nome:string,ativo:boolean,email:string,role:string
```
### Criando migração
```
npx sequelize-cli db:migrate
```
### Entrando na tabela
```
use escola_ingles;
```
### Mostrando tabelas
```
show tables;
```
### Mostrando tabela Pessoas
```
describe Pessoas;
```
### Criando linha na tabela Pessoas
```
insert into Pessoas (nome, ativo, email, role, createdAt, updatedAt) values ("Carla Gomes", 1, "carla@carla.com", "estudante", NOW(), NOW());
```
### Mostrando tudo na tabela Pessoas
```
select * from Pessoas;
```
### Criando seeder 
```
npx sequelize-cli seed:generate --name demo-pessoa
```
### Enviando dados para o banco
```
npx sequelize-cli db:seed:all
```
### Criando tabela Níveis
```
npx sequelize-cli model:create --name Niveis --attributes descr_nivel:string
```
### Criando tabela Turmas
```
npx sequelize-cli model:create --name Turmas --attributes data_inicio:dateonly
```
### Criando tabela Matrículas
```
npx sequelize-cli model:create --name Matriculas --attributes status:string
```
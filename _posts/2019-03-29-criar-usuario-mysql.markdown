---
layout: post
title:  "Criar usuário no MySql"
date:   2019-03-19 22:10:00 -0300
categories: My SQL
---
### Motivação:
È necessário criar um usuário no mysql geralmente quando não se usa uma ferramenta pronta como XAMPP,
ou para poder ter controle das premissões.

### Criando o User:
Com o mysql já instalado acesse o terminal com o comando `$ mysql `  
Agora crie o usuário:  
`mysql> CREATE USER 'NOVOUSER'@'LOCALHOST' IDENTIFIED BY 'PASSWORD'; `  

### Fornecer os privilégios:  
Agora é necessário fornecer os privilégios ao novo user, com o comando:  
`mysql> GRANT ALL PRIVILEGIES ON *.* TO 'NOVOUSER'@'LOCALHOST'; `  

#### Recarregar os privilégios:
Pronto agora basta recarregar os privilégios do seu usuário:  
`mysql> FLUSH PRIVILEGIES`  

### Acessar o seu usuário:  
Para acessar o my sql digite :
`$ mysql -u USER -p `  
Após digite sua senha e pronto!



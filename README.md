# WEB2-N1

## A senha de login permanece o padrão 
Usuario: admin 
Senha: admin

## Projeto de Eventos

Este é um projeto de eventos que é composto por frontend e backend desenvolvido em HTML/CSS e Java Spring Boot.

## Configurando o Banco de Dados

Para executar este projeto, você precisará iniciar um banco de dados MySQL e executar o seguinte script:

```sql
CREATE USER 'eron'@localhost IDENTIFIED BY 'eron' ;

CREATE DATABASE evento ;

GRANT ALL ON evento.* TO 'eron' @localhost

    WITH GRANT OPTION ;
    
FLUSH PRIVILEGES ;

use evento ;

create table evento (

id bigint not null auto_increment ,

agencia varchar ( 150 ) not null,

nome varchar ( 150 ) not null ,

data varchar ( 150 ) not null ,

local varchar ( 150 ) not null ,

primary key ( id )
) ;

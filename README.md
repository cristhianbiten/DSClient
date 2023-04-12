# DSClient
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/cristhianbiten/dsclient/blob/main/LICENSE) 

# Sobre o projeto


Projeto desenvolvido para o desafio do módulo de CRUD do Bootcamp Spring da DevSuperior.

A aplicação consiste em um CRUD de clientes, onde será possivel realizar buscas paginadas, busca por id, inserir novo recurso, atualizar recurso e deleter recurso.

## Modelo conceitual
![Modelo Conceitual](https://github.com/cristhianbiten/assets/blob/main/dsclient.png)

# Tecnologias utilizadas
## Back end
- Java
- Spring Boot
- JPA / Hibernate
- Maven
- H2

# Como executar o projeto

## Back end
Pré-requisitos: Java 17

[Tutorial de instalação Java](https://www.youtube.com/watch?v=QekeJBShCy4)

```bash
# Clonar repositório
git clone https://github.com/cristhianbiten/dsclient.git

# Entrar na pasta do projeto dsclient
cd client

# Entrar na pasta do projeto back end
cd backend

# Executar o projeto
./mvnw spring-boot:run
```

## Testes manuais
Pré-requisitos: Postman

Collection do Postman
https://www.getpostman.com/collections/8f7f24addf4ecba59fc1

```bash
# Busca paginada de clientes
GET /clients?page=0&linesPerPage=6&direction=ASC&orderBy=name

# Busca de cliente por id
GET /clients/1

# Inserção de novo cliente
POST /clients
{
  "name": "Maria Silva",
  "cpf": "12345678901",
  "income": 6500.0,
  "birthDate": "1994-07-20T10:30:00Z",
  "children": 2
}

# Atualização de cliente
PUT /clients/1
{
  "name": "Maria Silvaaa",
  "cpf": "12345678901",
  "income": 6500.0,
  "birthDate": "1994-07-20T10:30:00Z",
  "children": 2
}

# Deleção de cliente
DELETE /clients/1
```

# Autor

Cristhian Bitencourt

https://www.linkedin.com/in/cristhian-bitencourt-588b3317a/

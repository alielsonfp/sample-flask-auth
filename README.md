# Flask User Authentication API

Esta é uma API para autenticação de usuários utilizando Flask e MySQL.

## Sobre o Projeto

O objetivo deste projeto é criar uma API para autenticação de usuários, permitindo o cadastro, login, logout, atualização e exclusão de usuários. A aplicação foi desenvolvida com Flask e MySQL e visa proporcionar uma base sólida para a implementação de autenticação de usuários em aplicações web.

## Funcionalidades

- Cadastro de novos usuários.
- Login de usuários.
- Logout de usuários.
- Visualizar informações de usuários.
- Atualizar informações de usuários.
- Deletar usuários (apenas usuários com permissão de administrador podem deletar outros usuários).

## Requisitos funcionais

- [✔] O usuário deve poder se cadastrar na aplicação.
- [✔] O usuário deve poder fazer login na aplicação.
- [✔] O usuário deve poder fazer logout na aplicação.
- [✔] O usuário deve poder visualizar suas próprias informações de usuário.
- [✔] O usuário deve poder atualizar suas próprias informações de usuário.
- [✔] O usuário deve poder deletar sua própria conta de usuário.
- [✔] Apenas usuários com permissão de administrador podem deletar outros usuários.

## Requisitos não-funcionais

- [✔] A aplicação deve responder em um tempo razoável para todas as operações CRUD.
- [✔] A aplicação deve garantir a segurança das senhas dos usuários utilizando hashing com bcrypt.

## Arquivos do Projeto

### `app.py`

Este arquivo contém a aplicação Flask que define as rotas e a lógica para as operações de autenticação de usuários.

### `models/user.py`

Este arquivo define a classe `User`, que representa um usuário e possui métodos para autenticação e manipulação de informações do usuário.

### `database.py`

Este arquivo contém a configuração do banco de dados SQLAlchemy.

### `docker-compose.yml`

Este arquivo contém a configuração do Docker Compose para executar o banco de dados MySQL em um contêiner Docker.

### `requirements.txt`

Este arquivo contém as dependências do projeto, incluindo Flask, Flask-SQLAlchemy, Flask-Login, entre outras.

## Como Executar

### Pré-requisitos

- Python 3.x
- Docker
- Docker Compose

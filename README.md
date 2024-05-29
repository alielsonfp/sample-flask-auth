# Flask User Authentication API

Esta é uma API para autenticação de usuários utilizando Flask e MySQL.

## Sobre o Projeto

O objetivo deste projeto é criar uma API para autenticação de usuários, permitindo o cadastro, login, logout, atualização e exclusão de usuários. A aplicação foi desenvolvida com Flask e MySQL e visa proporcionar uma base sólida para a implementação de autenticação de usuários em aplicações web.

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

### Clonando o Repositório

```bash
git clone https://github.com/seu_usuario/flask-user-authentication.git
cd flask-user-authentication

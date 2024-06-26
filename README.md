# Sistema de Gerenciamento de Usuários

O Sistema de Gerenciamento de Usuários é uma aplicação para registro, autenticação e gerenciamento de usuários, fornecendo funcionalidades como cadastro, login, logout, visualização, atualização e deleção de contas de usuário.

## Sobre o Projeto

Este projeto foi desenvolvido com o objetivo de praticar e aplicar os conceitos de desenvolvimento web utilizando Flask e Python. Ele oferece uma API para gerenciamento de usuários, permitindo operações como cadastro, login, logout, visualização, atualização e deleção de contas de usuário. O Sistema de Gerenciamento de Usuários foi criado como parte de um processo de aprendizado e aprimoramento das habilidades em desenvolvimento web com Flask.

### Objetivos do Projeto:
- Praticar os conceitos fundamentais de Flask e Python.
- Implementar operações CRUD (Create, Read, Update, Delete) em uma API RESTful para gerenciamento de usuários.
- Aprender sobre autenticação de usuários e autorização de acesso em aplicativos web.
- Explorar boas práticas de segurança, incluindo o armazenamento seguro de senhas utilizando hashing com bcrypt.

Este projeto pode ser utilizado como um exemplo de aplicação Flask para gerenciamento de usuários e serve como uma base sólida para expandir e aprimorar suas habilidades em desenvolvimento web com Python. Sinta-se à vontade para clonar o repositório, experimentar e adaptar o código de acordo com suas necessidades e objetivos de aprendizado.

## Funcionalidades
- Cadastro de novos usuários.
- Login de usuários.
- Logout de usuários.
- Visualização das próprias informações de usuário.
- Atualização da própria senha de usuário.
- Deleção de contas de usuários por administradores.

## Requisitos Funcionais
- [✔] O usuário deve poder se cadastrar na aplicação.
- [✔] O usuário deve poder fazer login na aplicação.
- [✔] O usuário deve poder fazer logout na aplicação.
- [✔] O usuário deve poder visualizar suas próprias informações de usuário.
- [✔] O usuário deve poder atualizar sua própria senha de usuário.
- [✔] O usuário pode visualizar informações de outros usuários.
- [✔] Apenas usuários com permissão de administrador podem deletar contas de outros usuários.

## Requisitos Não-Funcionais
- [✔] A aplicação deve responder em um tempo razoável para todas as operações CRUD.
- [✔] A aplicação deve garantir a segurança das senhas dos usuários utilizando hashing com bcrypt.

# Banco de Dados

O Sistema de Gerenciamento de Usuários utiliza o MySQL como banco de dados para armazenar as informações dos usuários. O MySQL é uma escolha popular devido à sua confiabilidade e escalabilidade. Ele é acessado e manipulado por meio do SQLAlchemy, uma biblioteca Python para interagir com bancos de dados SQL. O MySQL armazena dados dos usuários, incluindo nomes de usuário, senhas (armazenadas com segurança usando bcrypt) e funções de usuário. O MySQL é executado em um contêiner Docker para facilitar a configuração e garantir a portabilidade do ambiente de desenvolvimento.

### Docker

O Docker é uma plataforma de código aberto que permite criar, implantar e gerenciar aplicativos em contêineres. Os contêineres são unidades de software que empacotam todo o código e suas dependências, tornando as aplicações independentes do ambiente em que são executadas. O Docker Compose é uma ferramenta que permite definir e executar aplicativos multi-contêiner com facilidade.

O banco de dados MySQL é executado em um contêiner Docker para simplificar o processo de configuração e garantir a consistência do ambiente de desenvolvimento. O Docker Compose é utilizado para definir e configurar o ambiente de desenvolvimento, incluindo a execução do contêiner MySQL.

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
git clone https://github.com/alielsonfp/sample-flask-auth.git
```

## Configurando o Ambiente

1. Execute o Docker Compose para iniciar o banco de dados MySQL:
```bash
docker-compose up -d
```

2. Instale as dependências do Python:
```bash
pip install -r requirements.txt
```

3. Execute a aplicação Flask:
```bash
python app.py
```

Agora a API estará disponível em http://localhost:5000.


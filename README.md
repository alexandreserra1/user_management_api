# User Management API

## Descrição

Esta API permite a criação, listagem e login de usuários utilizando Python e SQLite. Inclui uma interface front-end simples para uma experiência de usuário mais agradável.

## Instalação

1. Clone o repositório:

    ```bash
    git clone <URL_DO_REPOSITORIO>
    cd user_management_api
    ```

2. Instale as dependências necessárias:

    ```bash
    pip install flask sqlite3 werkzeug
    ```

## Rotas

A API oferece as seguintes rotas:

* `/api/users`: Cria um novo usuário (POST)
    - Exemplo de requisição:
    ```json
    {
        "username": "example",
        "password": "password"
    }
    ```

* `/api/users`: Lista todos os usuários (GET)
* `/api/login`: Realiza login de um usuário (POST)
z- Exemplo de requisição:
    ```json
    {
        "username": "example",
        "password": "password"
    }
    ```

## Front-end

A interface front-end inclui três páginas:

* `/register`: Página de registro de usuários
* `/login`: Página de login de usuários
* `/users`: Página de listagem de usuários

## Banco de Dados

O banco de dados utilizado pelo projeto é SQLite. O banco de dados é armazenado no arquivo `database.db`, que está localizado no diretório raiz do projeto.

A tabela `users` do banco de dados contém as seguintes colunas:

* `id`: Identificador único do usuário (inteiro, auto-incrementado, chave primária)
* `username`: Nome de usuário do usuário (texto)
* `password`: Senha do usuário (texto, armazenada como hash)

## Gerenciador de Banco de Dados

Recomendo utilizar o SQLite Studio ou o DB Browser for SQLite para visualizar e editar o banco de dados.

## Licença

Este projeto está disponível sob a licença MIT.

## Executando o Projeto

Para executar o projeto, basta executar o comando:

python -m unittest tests

```bash
python app.py

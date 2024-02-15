# API Flask Conectada ao Banco de dados para Gerenciamento de Livros
Esta é uma API Flask com conexao em um Banco de dados SQLite para realizar operações CRUD (Create, Read, Update, Delete) em livros. A API utiliza Flask-RestPlus para facilitar a criação dos endpoints e Flask-Marshmallow para a serialização e desserialização dos objetos.

# Instalação
1. Clone o repositório:

   ```bash
   git clone https://github.com/Digao07/FLASK_SQLALCHEMY.git
   
2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   
3. Execute a aplicação:
   ```bash
   python app.py

## URL base 
A URL base para acessar esta API é localhost.

## Endpoints

### Obter Todos os Livros
- **URL**: `/api/books`
- **Método**: `GET`
- **Descrição**: Recupera todos os livros.

### Obter um Livro por ID
- **URL**: `/api/books/<id>`
- **Método**: `GET`
- **Descrição**: Recupera um livro pelo seu ID.

### Criar um Livro
- **URL**: `/api/books`
- **Método**: `POST`
- **Descrição**: Cria um novo livro.

### Atualizar um Livro
- **URL**: `/api/books/<id>`
- **Método**: `PUT`
- **Descrição**: Atualiza um livro existente.

### Deletar um Livro
- **URL**: `/api/books/<id>`
- **Método**: `DELETE`
- **Descrição**: Deleta um livro pelo seu ID.

## Modelos

### Livro
- **Atributos**:
  - `id` (inteiro): O identificador único do livro.
  - `title` (string): O título do livro.
  - `pages` (inteiro): O número de páginas do livro.

## Tratamento de Erros
- Os erros de validação são tratados e retornados com um código de status 400.

## Banco de Dados
- A aplicação utiliza o SQLite como banco de dados, com o nome do arquivo `data.db`.

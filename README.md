# Sistema de Gerenciamento de Biblioteca

Este projeto é um sistema simples de gerenciamento de biblioteca que utiliza SQLite para armazenar informações sobre autores, livros e empréstimos.

## Estrutura do Banco de Dados

O banco de dados contém três tabelas principais:

1. **Autores**
   - `AutorID`: ID do autor (chave primária).
   - `Nome`: Nome do autor.
   - `Nacionalidade`: Nacionalidade do autor.

2. **Livros**
   - `LivroID`: ID do livro (chave primária).
   - `Titulo`: Título do livro.
   - `AutorID`: ID do autor (chave estrangeira).
   - `AnoPublicacao`: Ano de publicação do livro.
   - `Genero`: Gênero do livro.

3. **Empréstimos**
   - `EmprestimoID`: ID do empréstimo (chave primária).
   - `LivroID`: ID do livro (chave estrangeira).
   - `DataEmprestimo`: Data do empréstimo.
   - `DataDevolucao`: Data da devolução.
   - `NomeUsuario`: Nome do usuário que fez o empréstimo.

## Como Executar o Projeto

1. **Clone o repositório:**

   ```bash
   git clone https://github.com/seuusuario/seurepositorio.git
   cd seurepositorio

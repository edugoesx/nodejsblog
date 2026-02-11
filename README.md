# NodeJs Blog

Um sistema de blog completo e funcional desenvolvido com **Node.js**, **Express** e **MongoDB**. O projeto oferece autenticação segura, painel administrativo e operações de CRUD para postagens, utilizando **EJS** para renderização front-end.

![Node.js](https://img.shields.io/badge/Node.js-v18+-green)

## Tecnologias Utilizadas

O projeto foi construído utilizando as seguintes bibliotecas e ferramentas:

- **Back-end:** Node.js, Express.js
- **Banco de Dados:** MongoDB (com Mongoose)
- **Template Engine:** EJS (com Express EJS Layouts)
- **Autenticação & Segurança:**
  - `bcryptjs` (Hash de senhas)
  - `jsonwebtoken` (Autenticação via Token JWT)
  - `cookie-parser` (Gerenciamento de cookies)
- **Outros:**
  - `dotenv` (Gerenciamento de variáveis de ambiente)
  - `method-override` (Suporte a métodos PUT/DELETE em formulários HTML)
  - `connect-mongo` (Session store no MongoDB)

## Funcionalidades

- ** Home Page:** Listagem das postagens mais recentes.
- ** Barra de Pesquisa:** Funcionalidade de busca para filtrar postagens por título ou conteúdo.
- ** Página do Post:** Leitura detalhada de um artigo específico.
- ** Autenticação Administrativa:**
  - Login seguro com verificação de JWT armazenado em Cookies.
  - Proteção de rotas administrativas (Middleware de verificação).
- **Painel de Admin (CRUD):**
  - **Criar:** Editor para novas postagens.
  - **Editar:** Atualização de conteúdo existente.
  - **Excluir:** Remoção de postagens.

## Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:
- [Node.js](https://nodejs.org/) (Versão 16 ou superior recomendada)
- [MongoDB](https://www.mongodb.com/) (Rodando localmente ou via MongoDB Atlas)
- Git

## Instalação e Configuração

1. **Clone o repositório:**
   
   git clone https://github.com/edugoesx/nodejsblog.git
   
   cd nodejsblog
   
**Instale as dependências:**
Execute o comando abaixo para instalar todas as bibliotecas necessárias:

npm install bcryptjs connect-mongo cookie-parser dotenv ejs express express-ejs-layouts jsonwebtoken method-override mongoose

**Configure as Variáveis de Ambiente:**
Crie um arquivo .env na raiz do projeto e adicione as seguintes chaves (ajuste os valores conforme seu ambiente)

MONGODB_URI=mongodb+srv://<usuario>:<senha>@cluster.mongodb.net/blog_db
JWT_SECRET=sua_chave_secreta_super_segura
PORT=3000

**Como Rodar:**
Para iniciar o servidor em ambiente de desenvolvimento (ou produção, dependendo do script configurado no package.json):

npm start

Acesse o projeto no navegador em: http://localhost:3000




Desenvolvido por Eduardo Goes

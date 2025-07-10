# API - Contact Manager 📒

![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)
![Tech](https://img.shields.io/badge/tech-Node.js%20%26%20Express-68A063?logo=node.js)

A RESTful API for a personal contact management system. Built with Node.js, Express, and Prisma, it allows users to register, log in, and securely manage their own list of contacts.

## ✨ Features

-   **Full User Management:** Complete CRUD operations for user accounts.
-   **Personal Contact Book:** Full CRUD for contacts (create, read, update, delete), linked to the logged-in user.
-   **Secure Authentication:** User login system using JWT to grant access.
-   **Protected Routes:** Ensures that a user can only access and manage their own contacts.
-   **Secure Password Storage:** Passwords are encrypted using `bcrypt`.
-   **Data Validation:** Uses Zod to validate input data and ensure integrity.

## 🛠️ Tech Stack

-   **Runtime:** [Node.js](https://nodejs.org/)
-   **Framework:** [Express.js](https://expressjs.com/pt-br/)
-   **Language:** [TypeScript](https://www.typescriptlang.org/)
-   **ORM:** [Prisma](https://www.prisma.io/)
-   **Database:** [PostgreSQL](https://www.postgresql.org/)
-   **Authentication:** [JSON Web Token (JWT)](https://jwt.io/) & [Bcrypt](https://www.npmjs.com/package/bcrypt)
-   **Schema Validation:** [Zod](https://zod.dev/)

## 🚀 Getting Started

To run this project locally, you'll need Node.js, npm, and a running PostgreSQL instance.

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/rafabt-hub/api-rest-project.git
    ```
2.  **Navigate to the project directory:**
    ```sh
    cd api-rest-project
    ```
3.  **Install dependencies:**
    ```sh
    npm install
    ```
4.  **Set up environment variables:**
    Create a `.env` file in the root directory and add your database connection string and JWT secret.
    ```.env
    DATABASE_URL="postgresql://USER:PASSWORD@HOST:PORT/DATABASE"
    JWT_SECRET="your-super-secret-key"
    ```
    *Replace the values with your PostgreSQL credentials and a secret key of your choice.*

5.  **Run database migrations:**
    This will create the necessary tables in your database.
    ```sh
    npx prisma migrate dev
    ```
6.  **Run the development server:**
    ```sh
    npm run dev
    ```
    The API will be available at `http://localhost:3000`.

## 📄 License

This project is licensed under the MIT License.

---

<details>
  <summary>🇧🇷 Ver em Português</summary>

  <br>

  > Uma API RESTful para um sistema de gerenciamento de contatos pessoais. Construída com Node.js, Express e Prisma, permite que usuários se cadastrem, façam login e gerenciem de forma segura sua própria lista de contatos.

  ### ✨ Funcionalidades

  -   **Gerenciamento de Usuários:** Operações CRUD completas para contas de usuário.
  -   **Agenda de Contatos Pessoal:** CRUD completo para contatos, vinculados ao usuário logado.
  -   **Autenticação Segura:** Sistema de login de usuário usando JWT para conceder acesso.
  -   **Rotas Protegidas:** Garante que um usuário só possa acessar e gerenciar seus próprios contatos.
  -   **Armazenamento Seguro de Senhas:** Senhas são criptografadas com `bcrypt`.
  -   **Validação de Dados:** Usa Zod para validar os dados de entrada e garantir a integridade.

  ### 🚀 Como Executar

  Para rodar este projeto, você precisará do Node.js, npm e uma instância do PostgreSQL ativa.

  1.  **Clone o repositório.**
  2.  **Navegue até a pasta do projeto.**
  3.  **Instale as dependências:** `npm install`.
  4.  **Configure as variáveis de ambiente:** Crie um arquivo `.env` na raiz e adicione sua string de conexão do banco e um segredo para o JWT.
  5.  **Execute as migrações do banco:** `npx prisma migrate dev`.
  6.  **Inicie o servidor:** `npm run dev`. A API estará rodando em `http://localhost:3000`.

</details>

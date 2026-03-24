# 📚 API Biblioteca

API REST desenvolvida com .NET para gerenciamento de uma biblioteca, permitindo operações de cadastro, consulta, atualização e remoção de dados.

---

## 🚀 Tecnologias utilizadas

* .NET 8
* ASP.NET Core
* Entity Framework Core
* SQL Server
* DotNetEnv

---

## 📁 Estrutura do projeto

* Controllers → Endpoints da API
* Services → Regras de negócio
* Models → Entidades do sistema
* Data → Contexto e configurações do banco

---

## ⚙️ Como rodar o projeto

### ✅ Pré-requisitos

* .NET 8 instalado
* SQL Server (local ou remoto)

---

### 🔐 Configuração das variáveis de ambiente

Este projeto utiliza um arquivo `.env` para armazenar dados sensíveis.

1. Copie o arquivo `.env.example`:

```bash
cp .env.example .env
```

2. Preencha com sua connection string:

```env
ConnectionStrings__DefaultConnection=Server=SEU_SERVIDOR;Database=ApiBiblioteca;Trusted_Connection=True;TrustServerCertificate=True;
```

---

### 🗄️ Rodar as migrations

```bash
dotnet ef database update
```

---

### ▶️ Executar a aplicação

```bash
dotnet run
```

---

## 📌 Endpoints principais

| Método | Rota             | Descrição             |
| ------ | ---------------- | --------------------- |
| GET    | /api/livros      | Lista todos os livros |
| GET    | /api/livros/{id} | Busca livro por ID    |
| POST   | /api/livros      | Cadastra novo livro   |
| PUT    | /api/livros/{id} | Atualiza livro        |
| DELETE | /api/livros/{id} | Remove livro          |

---

## 🔐 Segurança

Este projeto segue boas práticas de segurança:

* Uso de variáveis de ambiente (`.env`)
* Arquivo `.env` não versionado
* Arquivo `.env.example` para referência
* Nenhuma informação sensível exposta no repositório

---

## 🧠 Aprendizados

Este projeto foi desenvolvido com foco em:

* Construção de APIs REST
* Boas práticas com Entity Framework
* Organização em camadas
* Configuração segura de credenciais

---

## 📄 Licença

Este projeto é para fins de estudo.

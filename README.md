

# 🧠 Projeto de Apoio à Recuperação do Alcoolismo – Backend

Este é o repositório backend do projeto desenvolvido para a disciplina Mundo II, com foco em oferecer suporte, acompanhamento e integração de responsáveis/cuidadores para pessoas em recuperação do alcoolismo.

## 🛠️ Tecnologias Utilizadas

- [NestJS](https://nestjs.com/) – Framework Node.js para aplicações escaláveis
- [Prisma ORM](https://www.prisma.io/) – ORM moderno e poderoso
- [SQLite](https://www.sqlite.org/index.html) – Banco de dados leve e embutido
- [TypeScript](https://www.typescriptlang.org/) – Tipagem estática para JavaScript

## 📦 Instalação

### 1. Clone o repositório

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
````

### 2. Instale as dependências

```bash
npm install
```

### 3. Configure o banco de dados SQLite

Verifique o arquivo `.env` (já incluído no projeto):

```env
DATABASE_URL="file:./dev.db"
```

### 4. Rode as migrações do Prisma

```bash
npx prisma migrate dev --name init
```

> Isso criará o arquivo `dev.db` com as tabelas necessárias.

### 5. Inicie o servidor

```bash
npm run start:dev
```

A API estará disponível em:
🔗 `http://localhost:3000`

---

## 📁 Estrutura de Pastas

```
src/
├── app.module.ts
├── main.ts
├── user/
│   ├── user.controller.ts
│   ├── user.service.ts
│   └── user.module.ts
├── recovery/
│   └── ... (acompanhamento da recuperação)
prisma/
└── schema.prisma
```

> **Nota**: A estrutura pode variar conforme os domínios do sistema (usuário, cuidador, paciente, etc.).

---

## 🔍 Funcionalidades

* Cadastro e gerenciamento de usuários (pessoas em recuperação, responsáveis/cuidadores)
* Registro de atividades ou relatos de acompanhamento
* Consulta e atualização de progresso
* Integração com cuidadores/responsáveis
* Controle de acesso básico

---

## 🧪 Testes

> (Opcional – adicione se houver testes implementados)

```bash
npm run test
```

---

## 📌 Observações

* Este projeto é **acadêmico**, mas estruturado seguindo boas práticas de arquitetura limpa com NestJS.
* O banco de dados **SQLite** foi escolhido por simplicidade e portabilidade durante o desenvolvimento.

---

## 🤝 Colaboradores

* Lucas (Igara/Igarassu) – Back-end Developer
* Ygor Fellipe Nogueira
* Maria Luiza Vidal

---

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

---

# API NODEJS SOLID
API feito em NodeJS durante as aulas de SOLID da Rocketseat

<br>

## 💻 Tecnologias Utilizadas nesse Projeto
<div style="display: inline_block">
  <img align="center" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/fastify/fastify-original.svg">
  <img align="center" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg">
  <img align="center" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original-wordmark.svg">
  <img align="center" height="50" width="60" src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/docker/docker-original-wordmark.svg">
</div>

<br>

## RFs (Requisitos funcionais)
- [x] Deve ser possível se cadastrar;
- [x] Deve ser possível se autenticar;
- [x] Deve ser possível obter o perfil de um usuário logado;
- [x] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [x] Deve ser possível o usuário obter o seu histórico de check-ins;
- [x] Deve ser possível o usuário buscar academias próximas (até 10km);
- [x] Deve ser possível o usuário buscar academias pelo nome;
- [x] Deve ser possível o usuário realizar check-in em uma academia;
- [x] Deve ser possível validar o check-in de um usuário;
- [x] Deve ser possível cadastrar uma academia;

<br>

## RNs (Regras de negócio)
- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [x] O usuário não pode fazer 2 check-ins no mesmo dia;
- [x] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [x] O check-in só pode ser validado até 20 minutos após ser criado;
- [x] O check-in só pode ser validado por administradores;
- [x] A academia só pode ser cadastrada por administradores;

<br>

## RNFs (Requisitos não-funcionais)
- [x] A senha do usuário precisa estar criptografada;
- [x] Os dados da aplicação precisam estar persistidos em um banco PostgreSQL;
- [x] Todas listas de dados precisam estar paginadas com 20 itens por página;
- [x] O usuário deve ser identificado por um JWT (JSON Web Token);

<br>

## Especificações
- Node: 20.14.0
- Pacote de Gerenciamento de Dependências: NPM
- Framework: Fastify

<br>

## Observações
Necessário configurar um arquivo .env antes de rodar o projeto
```bash
NODE_ENV=dev
PORT=3333
DATABASE_URL="postgresql://docker:docker@localhost:5432/apisolid?schema=public"
JWT_SECRET=ff47b44933a81ba5bdf823cdda59eb7f825bc4f34c86111fee15283c1cce21b1
```

<br>

## Como instalar as dependências
```bash
$ npm install
```

<br>

## Rodar o Projeto
```bash
$ npm run dev
```

<br>

## Rodar os Testes
```bash
$ npm run test:e2e
```
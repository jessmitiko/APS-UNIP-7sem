# APS-UNIP-7sem

[![Build Status](https://travis-ci.com/ogabriel/APS-UNIP-7sem.svg?branch=master)](https://travis-ci.com/ogabriel/APS-UNIP-7sem)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)

# O que é uma APS? [Um teste x]

APS, ou, Atividade Prática Supervisionada, é um exercício em grupo feito semestralmente pelos alunos da instituição de ensino UNIP. O tema, indiferente do curso que está sendo prestado, está sempre ligado a soluções sustentáveis ou ao meio ambiente.
No caso do curso que eu presto, Ciência da computação, além do trabalho escrito, tem de ser entregue uma aplicação, cujo os requisitos são ditados pelo coordenador do curso.

Este trabalho também possui uma parte [escrita](https://github.com/ogabriel/APS-UNIP-7sem-doc).

## Qual a proposta desse semestre?

Criar um sistema para o monitoramento de árvores e plantas pelo mundo, podendo gerenciar compensação de carbono feita pelas empresas e árvores plantadas por usuários comúns voluntários.

## Requerimentos

- nodejs (>=10.20.1)
- postgres (>= 10)
- postgis (>=2.4)
- acesso a internet (por causa do leaflet)

## Instruções:

1. Tenha uma versão de nodejs compatível (12.x.x é recomendável)
2. Instale as dependências com `npm install`
3. Copie o `.env.sample` para `.env`
4. Modifique o arquivo `.env` para as configurações do seu setup
5. Crie o banco de dados com `npx sequelize db:create` ou `npm run db:create`
6. Migrar o banco de dados com `npx sequelize db:migrate` ou `npm run db:migrate`
7. Para popular o banco de dados use `npx sequelize db:seed:all` ou `npm run db:seed`
8. Para dar start no server (localmente) use `npm run dev`

## TODO

- adicionar campo de pesquisa na página principal (com um botão de criar árvores e configurações)
- adicionar página de login
- adicionar página de criar usuário (comúm e empresa)
- adicionar página de criação de árvore

## APIs

- /api
  - /v1
    - /users
      - GET /users/:id
      - POST /users/:id (create)
      - PUT /users/:id (update)
    - /companies
      - GET /companies/
    - /trees
      - GET /trees
      - GET /trees/:id
      - POST /trees/:id (create)
      - PUT /trees/:id (update)

## Tecnologias a serem usadas

- nodejs
- leaflet
- OpenStreetMap
- express
- sequelize
- postgreSQL (with Postgis)
- passport

## APSs anteriores:

- **APS 2º semestre de 2019:** [Sistema de autenticação biométrica](https://github.com/ogabriel/APS-UNIP-6sem)
- **APS 1º semestre de 2019:** [Comunicação em rede através de WebSocket](https://github.com/ogabriel/APS-UNIP-5sem)
- **APS 2º semestre de 2018:** [Apresentar 3 tipos de Sort Diferentes](https://github.com/ogabriel/APS-UNIP-4sem)
- **APS 1º semestre de 2018:** [Programa console sobre sustentabilidate](https://github.com/ogabriel/APS-UNIP-3sem)
- **APS 2º semestre de 2017:** [Cifra de César](https://github.com/ogabriel/APS-UNIP-2sem)
- **APS 1º semestre de 2017:** [Site sobre cidades sustentáveis](https://github.com/ogabriel/APS-UNIP-1sem)

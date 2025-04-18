# 📚 Plataforma de Gestão de Cursos e Matrículas

Este projeto simula uma plataforma educacional com arquitetura baseada em microsserviços, dividida em dois serviços principais: **Cursos** e **Matrículas**. Desenvolvido em Java com Spring Boot, o sistema oferece funcionalidades completas para o gerenciamento de cursos e alunos, além da matrícula de estudantes.

---

## 🔍 Visão Geral

A aplicação foi construída com foco em boas práticas de desenvolvimento, comunicação entre serviços e testes. Os microsserviços se comunicam via HTTP utilizando o OpenFeign e seguem uma arquitetura enxuta e escalável. Entre as principais funcionalidades estão:

- 📌 Cadastro, inativação e listagem de cursos e alunos
- 🔁 Regras de negócio como:
  - Limite de alunos por curso
  - Inativação em cascata (curso → matrículas)
  - Reativação condicional de matrículas
- 📑 Documentação interativa via Swagger
- ✅ Testes unitários com cobertura relevante

---

## 🛠 Tecnologias Utilizadas

- Java 17
- Spring Boot (Web, Data JPA)
- OpenFeign
- SpringDoc Swagger
- H2 Database
- Lombok
- JUnit 5
- ModelMapper

---

## 🗂 Repositórios

Este projeto é dividido em dois microsserviços, disponíveis nos seguintes repositórios:

| Microsserviço | Repositório                                                                   |
| ------------- | ----------------------------------------------------------------------------- |
| Cursos        | [Time-7-Desafio02/cursos](https://github.com/Time-7-Desafio02/cursos)         |
| Matrículas    | [Time-7-Desafio02/matriculas](https://github.com/Time-7-Desafio02/matriculas) |

---

## 🚀 Como executar localmente

Cada serviço pode ser executado separadamente utilizando Spring Boot. Recomenda-se executar os dois simultaneamente para permitir comunicação via Feign Client.

1. Clone os dois repositórios
2. Execute ambos os projetos (`cursos` na porta 8080 e `matriculas` na 8081)
3. Acesse o Swagger de cada serviço:

- Cursos: [http://localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)
- Matrículas: [http://localhost:8081/swagger-ui.html](http://localhost:8081/swagger-ui.html)

---

## 👥 Equipe

Projeto desenvolvido pelo **Time 7**:

- Elias Mathias Sand
- João Pedro Golenia
- Jonas Roberto Leandro
- Lucas Henrique Teixeira Ribeiro

Durante o **Desafio 02** da formação Java Backend da [Compass UOL](https://compass.uol/).

---

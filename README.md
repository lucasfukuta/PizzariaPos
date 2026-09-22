# 🍕 Pizzaria POS

API REST desenvolvida como atividade acadêmica da **Pós-Graduação em Desenvolvimento Full Stack do UniCEUB**.

O projeto teve como objetivo aplicar conceitos de desenvolvimento backend utilizando **C#, .NET 8, ASP.NET Core e Entity Framework Core**, simulando a estrutura inicial de um sistema de gerenciamento para uma pizzaria.

---

## 📚 Contexto acadêmico

Este projeto foi desenvolvido durante a **Pós-Graduação em Desenvolvimento Full Stack do Centro Universitário de Brasília (UniCEUB)**, como atividade prática para aplicação dos conhecimentos relacionados ao desenvolvimento de APIs e ao ecossistema .NET.

A proposta consistiu na construção de uma API para uma aplicação de pizzaria, explorando conceitos como:

* Desenvolvimento de APIs REST;
* Arquitetura de aplicações .NET;
* Entity Framework Core;
* Injeção de Dependência;
* Repository Pattern;
* Persistência de dados;
* Documentação de APIs com Swagger/OpenAPI.

---

## 🎯 Objetivo

O objetivo do projeto foi desenvolver uma API backend capaz de servir como base para um sistema de gerenciamento de uma pizzaria.

A aplicação foi estruturada para trabalhar principalmente com **pizzas e estoque**, utilizando o Entity Framework Core para acesso aos dados.

O projeto também serviu como exercício prático para consolidar conhecimentos de **C# e ASP.NET Core** adquiridos durante a pós-graduação.

---

## 🛠️ Tecnologias utilizadas

* **C#**
* **.NET 8**
* **ASP.NET Core Web API**
* **Entity Framework Core**
* **Entity Framework Core InMemory**
* **Swagger / OpenAPI**
* **Git**

---

## 🏗️ Estrutura do projeto

A solução está organizada em um projeto principal de API:

```text
PizzariaPos/
│
├── Pizza.API/
│   │
│   ├── Controllers/
│   │
│   ├── Persistence/
│   │   ├── PizzaRepository
│   │   └── EstoqueRepository
│   │
│   ├── Program.cs
│   ├── appsettings.json
│   └── Pizza.API.csproj
│
├── Pizzaria.sln
├── .gitignore
└── .gitattributes
```

A separação entre controllers e camada de persistência foi utilizada para organizar as responsabilidades da aplicação e facilitar sua evolução.

---

## 🔌 API REST

A aplicação foi desenvolvida utilizando **ASP.NET Core Web API**.

A API possui integração com **Swagger/OpenAPI**, permitindo visualizar e testar os endpoints disponibilizados pela aplicação.

Após executar o projeto, a documentação pode ser acessada através de:

```text
/swagger
```

O Swagger permite realizar requisições diretamente pela interface web, facilitando o processo de desenvolvimento e testes da API.

---

## 💾 Persistência de dados

O projeto utiliza **Entity Framework Core** como ORM e, para a atividade acadêmica, foi utilizado o provider **InMemory**.

```csharp
builder.Services.AddDbContext<PizzaDbContext>(
    options => options.UseInMemoryDatabase("pizza")
);
```

A utilização do banco em memória permite executar a aplicação sem a necessidade de configurar um servidor de banco de dados externo.

> **Nota:** por utilizar um banco de dados em memória, os dados não possuem persistência permanente entre execuções da aplicação.

---

## 🚀 Como executar

### Pré-requisitos

Para executar o projeto, é necessário ter instalado:

* [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)
* Git
* Uma IDE compatível com .NET, como Visual Studio, Visual Studio Code ou JetBrains Rider

### 1. Clone o repositório

```bash
git clone https://github.com/lucasfukuta/PizzariaPos.git
```

### 2. Acesse o diretório

```bash
cd PizzariaPos
```

### 3. Restaure as dependências

```bash
dotnet restore
```

### 4. Execute a API

```bash
dotnet run --project Pizza.API
```

### 5. Acesse o Swagger

Com a aplicação em execução, acesse:

```text
https://localhost:<porta>/swagger
```

A porta utilizada pode variar de acordo com a configuração do ambiente de execução.

---

## 🧠 Conceitos praticados

Durante o desenvolvimento foram aplicados conceitos importantes do ecossistema .NET, incluindo:

### ASP.NET Core

Utilização do framework para criação de uma API REST e configuração da aplicação.

### Entity Framework Core

Utilização de ORM para abstração do acesso aos dados.

### Dependency Injection

Utilização do mecanismo nativo de injeção de dependência do ASP.NET Core para disponibilizar os serviços e repositórios utilizados pela aplicação.

### Repository Pattern

Organização do acesso aos dados através de repositories, separando essa responsabilidade dos controllers.

### Swagger / OpenAPI

Documentação interativa da API para facilitar testes e exploração dos endpoints.

---

## 📖 Finalidade do projeto

Este projeto possui **finalidade acadêmica e educacional**.

Ele representa uma das atividades práticas realizadas durante minha formação em **Desenvolvimento Full Stack no UniCEUB** e faz parte da minha trajetória de aprendizado no ecossistema **C#/.NET**.

O código também é mantido como parte do meu portfólio para demonstrar conhecimentos adquiridos durante a formação.

---

## 🔮 Possíveis evoluções

Como exercício acadêmico, a aplicação possui espaço para futuras melhorias, como:

* [ ] Utilização de banco de dados relacional;
* [ ] Implementação completa de CRUD;
* [ ] Gerenciamento de pedidos;
* [ ] Cadastro de clientes;
* [ ] Gerenciamento de ingredientes;
* [ ] Controle de estoque;
* [ ] Autenticação e autorização;
* [ ] DTOs;
* [ ] Validação de dados;
* [ ] Tratamento global de exceções;
* [ ] Testes unitários;
* [ ] Testes de integração;
* [ ] Containerização com Docker;
* [ ] Pipeline de CI/CD;
* [ ] Desenvolvimento de uma interface frontend.

---

## 👨‍💻 Autor

### Lucas Fukuta

Desenvolvedor com interesse em **C#, .NET, desenvolvimento backend, aplicações web e Inteligência Artificial**.

Este projeto foi desenvolvido como parte da **Pós-Graduação em Desenvolvimento Full Stack — UniCEUB**.

## 📄 Licença

Projeto desenvolvido para fins **acadêmicos e educacionais**.

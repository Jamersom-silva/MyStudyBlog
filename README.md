# 📘 StudyBlog — Blog pessoal de jornada de estudos

O **StudyBlog** é um projeto full-stack criado para documentar, de forma pública, minha jornada de estudos em tecnologia (Java, Spring, Backend, etc.), funcionando como um **blog técnico pessoal**, com organização por tópicos e roadmap de aprendizado.

O projeto foi pensado como um **MVP realista**, focado em boas práticas de backend, segurança e arquitetura, simulando um sistema que poderia ser utilizado em produção.

---

## 🎯 Objetivo do projeto

- Registrar e compartilhar minha evolução técnica
- Organizar conteúdos por **tópicos** (ex: Java, Spring, SQL)
- Exibir um **roadmap visual** do que já foi estudado
- Permitir **postagens apenas pelo administrador**
- Servir como **projeto de portfólio** para vagas backend Java

---

## 🧩 Funcionalidades

### 🔓 Público
- Visualizar lista de posts publicados
- Ler post completo por slug
- Visualizar tópicos de estudo
- Visualizar roadmap de aprendizado por tópico

### 🔐 Admin (somente o autor)
- Login com autenticação JWT
- Criar posts em rascunho
- Publicar / despublicar posts
- Criar e gerenciar tópicos
- Criar e atualizar itens do roadmap

---

## 🛠️ Stack utilizada

### Backend
- **Java 17**
- **Spring Boot 3**
- **Spring Web**
- **Spring Data JPA (Hibernate)**
- **Spring Security + JWT**
- **Flyway** (versionamento de banco)
- **PostgreSQL**
- **Maven**

### Frontend (em desenvolvimento)
- **Angular** (standalone components)
- Consumo via API REST

---

## 🗂️ Arquitetura

O backend segue uma arquitetura em camadas:

Com separação clara de responsabilidades:
- Controllers: camada HTTP
- Services: regras de negócio
- Repositories: acesso a dados
- DTOs: contratos de entrada/saída
- Security: autenticação e autorização JWT

---

## 🔐 Segurança

- Autenticação baseada em **JWT**
- Rotas públicas e privadas bem definidas
- `/api/public/**` → acesso livre
- `/api/admin/**` → requer token JWT
- Sessão **stateless** (padrão REST)

---

## 🗄️ Banco de dados

- **PostgreSQL**
- Versionamento com **Flyway**
- Criação automática do schema ao iniciar a aplicação
- Controle total do modelo via migrations SQL

---

**DEPLOY** -> em breve 

# 🍔 API Delivery - 7º Termo (Template)

Repositório base para a disciplina de Arquitetura Orientada a Serviços (SOA). Este projeto é uma API RESTful desenvolvida com Spring Boot e conteinerizada com Docker, utilizando o GitHub Codespaces como ambiente de desenvolvimento padronizado.

## 🚀 Tecnologias Utilizadas
* **Java 17**
* **Spring Boot 4.0.3** (Spring Web, Spring Data JPA, MySQL Driver, Validation e Lombok)
* **MySQL 8** (via Docker)
* **Maven** (Gerenciador de Dependências)
* **GitHub Codespaces** (Ambiente de Desenvolvimento na Nuvem)

## 🛠️ Como usar este Template

1. Clique no botão verde **"Use this template"** (no topo da página) e selecione "Create a new repository".
2. Dê um nome ao seu repositório e clique em "Create".
3. No seu novo repositório, clique no botão verde **"Code"**, vá na aba **"Codespaces"** e clique em **"Create codespace on main"**.
4. Aguarde o ambiente carregar. O VS Code abrirá diretamente no seu navegador com o Java e o banco de dados MySQL já configurados e rodando.

## 🏃‍♂️ Como rodar o projeto

No terminal do Codespaces, utilize o Maven Wrapper para baixar as dependências e iniciar o servidor Spring:

```bash
# 1. Compilar o projeto e baixar dependências
./mvnw clean install -DskipTests
    # 1.1 Se der erro de permissão execute o comando abaixo no terminal e depois retorne ao passo 1
    chmod +x mvnw
    
# 2. Iniciar a aplicação Spring
./mvnw spring-boot:run
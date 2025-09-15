# API de Clientes - Spring Boot

Este projeto é uma API RESTful para gerenciamento de clientes, desenvolvida em **Java 17** com **Spring Boot**.  
Foi criado para praticar **Programação Orientada a Objetos, boas práticas de arquitetura e desenvolvimento backend**.

## 🚀 Funcionalidades
- Cadastro de clientes
- Listagem de todos os clientes
- Atualização de informações
- Exclusão de registros
- Banco de dados em memória (**H2**)

## 🔧 Tecnologias
- Java 17
- Spring Boot
- Spring Data JPA
- H2 Database
- Maven

## 📌 Endpoints principais
- `GET /clientes`
- `GET /clientes/{id}`
- `POST /clientes`
- `PUT /clientes/{id}`
- `DELETE /clientes/{id}`

## ▶️ Como executar
```bash
# clonar repositório
git clone https://github.com/alcantara-roberto/springboot-api-clientes.git
cd springboot-api-clientes

# executar o projeto
./mvnw spring-boot:run
```

A API estará disponível em: `http://localhost:8080/clientes`

## 💡 Observação
Este projeto simples demonstra conhecimentos e técnicas em **Java + Spring Boot + POO**.

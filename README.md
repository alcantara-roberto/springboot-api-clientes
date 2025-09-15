# API de Gerenciamento de Clientes

API RESTful para gerenciamento de clientes, desenvolvida como parte de um portfólio de projetos para demonstrar habilidades em desenvolvimento backend com **Java 17** e **Spring Boot**.

O projeto foca em boas práticas de arquitetura, desenvolvimento orientado a objetos e na criação de APIs coesas e eficientes.

## 🔧 Tecnologias Utilizadas
- **Java 17**
- **Spring Boot 3**
- **Spring Data JPA**
- **H2 Database** (Banco de dados em memória)
- **Maven**

## ✨ Recursos da API
- **CRUD Completo de Clientes:**
  - Cadastrar um novo cliente.
  - Listar todos os clientes.
  - Buscar um cliente por ID.
  - Atualizar os dados de um cliente existente.
  - Excluir um cliente.

## 📌 Endpoints

| Método HTTP | Endpoint           | Descrição                             |
|-------------|--------------------|---------------------------------------|
| `GET`       | `/clientes`        | Lista todos os clientes.              |
| `GET`       | `/clientes/{id}`   | Busca um cliente pelo seu ID.         |
| `POST`      | `/clientes`        | Cadastra um novo cliente.             |
| `PUT`       | `/clientes/{id}`   | Atualiza um cliente existente.        |
| `DELETE`    | `/clientes/{id}`   | Exclui um cliente.                    |

---

### Corpo da Requisição (Request Body)
Para os endpoints `POST` e `PUT`, o corpo da requisição deve ser um JSON com a seguinte estrutura:

```json
{
  "nome": "Seu Nome Completo",
  "email": "email@exemplo.com"
}
```

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
Antes de começar, você vai precisar ter instalado em sua máquina:
- [Git](https://git-scm.com)
- [Java Development Kit (JDK) 17](https://www.oracle.com/java/technologies/javase/jdk17-archive-downloads.html)

### Passos
```bash
# 1. Clone o repositório
git clone [https://github.com/alcantara-roberto/springboot-api-clientes.git](https://github.com/alcantara-roberto/springboot-api-clientes.git)

# 2. Acesse a pasta do projeto
cd springboot-api-clientes

# 3. Execute o projeto com o Maven Wrapper
./mvnw spring-boot:run
```
A API estará disponível para acesso em `http://localhost:8080/clientes`.

## 🗄️ Acessando o Banco de Dados (H2 Console)
O projeto utiliza um banco de dados em memória (H2) e o console para visualização está habilitado.

1.  Acesse o seguinte endereço no seu navegador:
    `http://localhost:8080/h2-console`

2.  Insira as seguintes informações para conectar:
    - **Driver Class**: `org.h2.Driver`
    - **JDBC URL**: `jdbc:h2:mem:clientesdb`
    - **User Name**: `sa`
    - **Password**: (deixe em branco)

Clique em **Connect** e você poderá visualizar a tabela `CLIENTE` e executar queries SQL.
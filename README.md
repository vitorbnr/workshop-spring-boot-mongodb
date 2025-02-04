# Workshop Spring Boot MongoDB 🚀
Este projeto foi desenvolvido como parte de um workshop prático, com o objetivo de demonstrar a integração entre Spring Boot e MongoDB, explorando conceitos de persistência de dados em bancos NoSQL. A aplicação consiste em uma API REST para gerenciamento de usuários e publicações.

## Tecnologias Utilizadas 💻

Java 17
Spring Boot 3
Spring Data 
MongoDB
Maven

## Como Executar 🚀
Para rodar o projeto localmente, siga os passos abaixo:

Clone o repositório:

```bash
git clone https://github.com/vitorbnr/workshop-spring-boot-mongodb.git
```

Navegue até o diretório do projeto:

```bash
cd workshop-spring-boot-mongodb
```

Compile e instale as dependências:

```bash
./mvnw clean install
```

Execute o MongoDB (caso ainda não esteja rodando):

```bash
docker run -d --name mongodb -p 27017:27017 mongo
```

Execute o projeto no terminal:

```bash
./mvnw spring-boot:run
```

Execute o projeto na IDE:

Abra sua IDE de preferÊncia.
Importe o projeto como Maven Project.
Execute a classe principal WorkshopmongoApplication.java.

## Instruções de Uso 📋

Rotas GET
/users → Retorna todos os usuários
/users/{id} → Retorna um usuário pelo ID
/posts → Retorna todas as publicações
/posts/{id} → Retorna uma publicação pelo ID

Rotas POST
/users → Cadastra um novo usuário
/posts → Cadastra uma nova publicação

Rotas PUT
/users/{id} → Atualiza um usuário existente
/posts/{id} → Atualiza uma publicação existente

Rotas DELETE
/users/{id} → Remove um usuário
/posts/{id} → Remove uma publicação

Conectando ao MongoDB
Caso queira acessar o banco MongoDB diretamente, utilize um cliente como MongoDB Compass ou conecte via terminal:

```bash
mongo
```

Para listar os bancos de dados disponíveis:

```bash
show dbs
```

Para acessar o banco usado pelo projeto:

```bash
use workshopdb
```
## Aprendizados 📚
Este projeto reforça os seguintes conceitos:

Desenvolvimento de APIs RESTful com Spring Boot.
Persistência de dados em banco NoSQL (MongoDB).
Modelagem de documentos e relacionamentos no MongoDB.
Boas práticas no desenvolvimento backend com Spring Data MongoDB.

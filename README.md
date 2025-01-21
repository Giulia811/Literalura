# 📚 Literalura - Explore o Universo dos Livros

**Encontre seus próximos livros favoritos!**

Literalura é um aplicativo para buscar e salvar informações sobre livros. Com uma integração robusta à API Gutendex, você pode explorar um banco de dados com milhares de títulos e armazenar os resultados para consultas futuras. Desenvolvido com Spring Boot e Java, o projeto utiliza PostgreSQL para gerenciamento de dados.

## ✨ Funcionalidades

- Pesquise livros pelo título com facilidade.
- Armazene os resultados de pesquisa em um banco de dados PostgreSQL.
- Consulte seus livros salvos a qualquer momento.

## 🛠️ Tecnologias Utilizadas

![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=java&logoColor=white) ![Spring](https://img.shields.io/badge/spring-%236DB33F.svg?style=for-the-badge&logo=spring&logoColor=white) ![GitHub](https://img.shields.io/badge/GitHub-%23121011.svg?style=for-the-badge&logo=github&logoColor=white) ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white) ![Apache Maven](https://img.shields.io/badge/Apache%20Maven-C71A36?style=for-the-badge&logo=Apache%20Maven&logoColor=white) ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJIDEA-000000.svg?style=for-the-badge&logo=intellij-idea&logoColor=white)

## ✅ Pré-requisitos

Antes de começar, certifique-se de ter instalado:

- **Java Development Kit (JDK) versão 11 ou superior**
- **Maven**
- **PostgreSQL**

## 🗄️ Configuração do Banco de Dados

1. Crie um banco de dados PostgreSQL.
2. Atualize as variáveis de ambiente necessárias:

   - `DB_HOST`: Host do banco de dados.
   - `DB_NAME`: Nome do banco de dados.
   - `DB_USER`: Usuário do banco de dados.
   - `DB_PASSWORD`: Senha do banco de dados.

3. As configurações no arquivo `application.properties` estão configuradas para usar variáveis de ambiente:

```properties
spring.application.name=literalura
spring.datasource.url=jdbc:postgresql://${DB_HOST}/${DB_NAME}
spring.datasource.username=${DB_USER}
spring.datasource.password=${DB_PASSWORD}
spring.datasource.driver-class-name=org.postgresql.Driver
```

## 🚀 Como Executar

1. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/literalura.git
   cd literalura
   ```

2. Compile e execute o projeto com Maven:

   ```bash
   mvn spring-boot:run
   ```

3. Acesse a aplicação em: [http://localhost:8080](http://localhost:8080)

## 📂 Estrutura do Projeto

```
src
├── main
│   ├── java/com/alura/literalura
│   │       ├── menu
│   │       ├── model
│   │       ├── repository
│   │       └── service
│   └── resources
│       └── application.properties
README.md
mvnw
mvnw.cmd
pom.xml
```

## 🙌 Créditos

- API Gutendex: [https://gutendex.com](https://gutendex.com)

# Academia Digital

Bem-vindo ao projeto **Academia Digital**. Este projeto consiste no desenvolvimento de uma API RESTful para modelar o sistema de uma academia de ginástica, utilizando Java e o framework Spring Boot.

## Objetivo do Projeto

O objetivo deste projeto é demonstrar a implementação de uma API RESTful que gerencia as operações básicas de uma academia, como cadastro de alunos, avaliação física e matrícula em atividades.

## Tecnologias Utilizadas

- Java 11
- Spring Boot
- Spring Data JPA
- Maven
- Banco de Dados H2 (em memória)

## Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:

- Java 11 ou superior
- Maven

## Configuração do Banco de Dados

O projeto utiliza o banco de dados H2, que roda em memória e não requer instalação. Para acessar o console do H2 enquanto a aplicação estiver rodando, utilize o seguinte endereço:

```
http://localhost:8080/h2-console
```

As configurações do banco estão no arquivo `application.properties`:

```properties
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.driverClassName=org.h2.Driver
spring.datasource.username=sa
spring.datasource.password=
spring.jpa.database-platform=org.hibernate.dialect.H2Dialect
spring.h2.console.enabled=true
```

## Executando a Aplicação

1. Clone este repositório:

   ```bash
   git clone https://github.com/jciterceros/academia-digital.git
   ```

2. Navegue até o diretório do projeto:

   ```bash
   cd academia-digital
   ```

3. Compile o projeto usando o Maven:

   ```bash
   mvn clean install
   ```

4. Execute a aplicação:

   ```bash
   mvn spring-boot:run
   ```

A aplicação estará disponível em `http://localhost:8080`.

## Estrutura do Projeto

O projeto segue a arquitetura padrão do Spring Boot:

- `src/main/java`: Contém o código-fonte da aplicação.
- `src/main/resources`: Contém os recursos estáticos e arquivos de configuração.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues e enviar pull requests.

## Licença

Este projeto está licenciado sob a licença MIT.


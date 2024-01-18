# README
## Link de Documentação

https://documenter.getpostman.com/view/18554860/2s9YsRdVYW

## Tecnologias usadas

- Java 17
- Maven
- Spring Boot 3
- Spring Cloud
- Domain Driven Development (DDD)

## Domain Driven Development (DDD)

DDD é um paradigma de design de software que enfatiza a importância do domínio do negócio no desenvolvimento de software. O objetivo é criar software que seja fácil de entender e manter, atendendo às necessidades do negócio.

## Abordagem do projeto

O projeto foi abordado utilizando DDD. O domínio do negócio foi modelado em classes e entidades, e a lógica de negócio foi implementada em serviços.

## Sandbox consumida

O projeto consome a seguinte sandbox:

[https://apisandbox.openbankproject.com/obp/v1.2.1/banks/rbs/accounts/savings-kids-john/public/transactions](https://apisandbox.openbankproject.com/obp/v1.2.1/banks/rbs/accounts/savings-kids-john/public/transactions)

Erro ao consumir a API:

Ao consumir a API, por vezes são retornados dados nulos ou o seguinte erro:

    {"code":400,"message":"OBP-50010: Scala return Empty box to Liftweb."}


Para evitar que essa situação afete a funcionalidade criada, foi implementado um mecanismo para criar dados em memória caso os dados retornados pela API sejam nulos.

## Comandos para rodar o projeto

Para rodar o projeto, execute os seguintes comandos:

```bash
mvn clean install
mvn spring-boot:run

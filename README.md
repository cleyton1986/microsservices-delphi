# microsservices-delphi
Repositório de exemplo microservice em delphi


[![Build Status](https://app.travis-ci.com/kyriosdata/exemplo.svg)](https://travis-ci.com/kyriosdata/exemplo)
[![SonarCloud Status](https://sonarcloud.io/api/project_badges/measure?project=com.github.kyriosdata%3Aexemplo&metric=alert_status)](https://sonarcloud.io/dashboard?id=com.github.kyriosdata%3Aexemplo)
[![Known Vulnerabilities](https://snyk.io/test/github/kyriosdata/exemplo/badge.svg?targetFile=pom.xml)](https://snyk.io/test/github/kyriosdata/exemplo)
[![Maven Central](https://maven-badges.herokuapp.com/maven-central/com.github.kyriosdata/exemplo/badge.svg)](https://maven-badges.herokuapp.com/maven-central/com.github.kyriosdata/exemplo)

# Escopo e objetivo

_Projeto que serve de referência para o desenvolvimento de software em Java_.

Ou seja, é um projeto proposto para ser clonado
e reutilizado no desenvolvimento dos seus projetos.

Este projeto inclui um conjunto "completo" de ferramentas, já configuradas, para o desenvolvimento
de software em Java.

Para ilustrar o projeto inclui:
(a) uma biblioteca formada por um único método que identifica o dia da semana para uma data fornecida;
(b) uma aplicação que oferece tal funcionalidade via linha de comandos e (c) uma RESTFul API ambas para acesso à funcionalidade da biblioteca.

> _Objetivo: ilustrar uma organização de código em Java usando
> "boas práticas" para inspirar projetos reais_.

## Iniciando...

- `git clone https://github.com/kyriosdata/exemplo`
- `cd exemplo`

Agora você poderá executar os vários comandos abaixo.

## Pré-requisitos

- `mvn --version`<br>
  você deverá ver a indicação da versão do Maven instalada e
  a versão do JDK, dentre outras. Observe que o JDK é obrigatório, assim como
  a definição das variáveis de ambiente **JAVA_HOME** e **M2_HOME**.

## Limpar, compilar, executar testes de unidade e cobertura

- `mvn clean`<br>
  remove diretório _target_

- `mvn compile`<br>
  compila o projeto, deposita resultados no diretório _target_

- `mvn test`<br>
  executa todos os testes do projeto. Para executar apenas parte dos testes, por exemplo,
  aqueles contidos em uma dada classe execute `mvn -Dtest=NomeDaClasseTest test`. Observe
  que o sufixo do nome da classe de teste é `Test` (padrão recomendado). Para executar um
  único teste `mvn -Dtest=NomeDaClasseTest#nomeDoMetodo test`.

- `mvn verify -P cobertura`<br>
  executa testes de unidade e produz relatório de
  cobertura em _target/site/jacoco/index.html_ além de verificar se limite mínimo
  de cobertura, conforme configurado, é satisfeito.

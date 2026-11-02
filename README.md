EcoDescarte

Projeto acadêmico desenvolvido para a AEP do 6º semestre de Engenharia de Software.

O EcoDescarte permite cadastrar e consultar pontos de coleta de resíduos, contribuindo para os ODS 11 e 12 da ONU.

Funcionalidades

Cadastrar, listar, pesquisar, editar e excluir pontos de coleta.

Buscar pontos por nome ou tipo de resíduo.

Cadastrar e gerenciar organizações responsáveis.

Acessar as funcionalidades pela interface web ou pela API REST.

Tecnologias

Java 21, Spring Boot, MongoDB, Maven, HTML, CSS e JavaScript.

Testes com JUnit, Mockito, MockMvc e JaCoCo.

Banco de dados

Na segunda entrega, o projeto passou a utilizar duas coleções MongoDB:

organizacoes: informações das organizações responsáveis.

pontos_coleta: dados dos pontos, endereço, resíduos aceitos e referência à organização.

A aplicação possui três pontos fictícios para demonstração.

Como executar

Pré-requisitos: Java 21, MongoDB, MongoDB Shell e Git.

No PowerShell, execute:

git clone https://github.com/PauloMalavasi/Aep-6-Semestre.git
cd .\Aep-6-Semestre
mongosh "mongodb://localhost:27017" --file .\6s\mongodb\init.js
cd .\6s
.\mvnw.cmd spring-boot:run

Acesse a aplicação em http://localhost:8080.

Documentação da API: http://localhost:8080/docs.

Testes e cobertura

Na pasta 6s, execute:

.\mvnw.cmd clean verify

Na validação documentada em 31/10/2026, o projeto apresentou:

65 testes Java aprovados.

99,23% de cobertura de instruções Java.

Cobertura superior aos 70% exigidos.

O relatório JaCoCo fica em 6s/target/site/jacoco/index.html, considerando a raiz do repositório.

Documentação

Diagramas

Resultados dos testes

Quadro de tarefas

Segunda entrega

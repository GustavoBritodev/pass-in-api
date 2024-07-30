
# Pass In API

[![Java](https://camo.githubusercontent.com/b0648ef7a9b6980ea27c1caaeb06d5c8503dbb4f9b4d9d7ca1df60a5edc14340/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6a6176612d2532334544384230302e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d6f70656e6a646b266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/b0648ef7a9b6980ea27c1caaeb06d5c8503dbb4f9b4d9d7ca1df60a5edc14340/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f6a6176612d2532334544384230302e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d6f70656e6a646b266c6f676f436f6c6f723d7768697465) [![Spring](https://camo.githubusercontent.com/c2a58428fe9b38967494da3b0a098f1d28f9cc395e3bbf123cbc14fb36bc1b07/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f737072696e672d2532333644423333462e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d737072696e67266c6f676f436f6c6f723d7768697465)](https://camo.githubusercontent.com/c2a58428fe9b38967494da3b0a098f1d28f9cc395e3bbf123cbc14fb36bc1b07/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f737072696e672d2532333644423333462e7376673f7374796c653d666f722d7468652d6261646765266c6f676f3d737072696e67266c6f676f436f6c6f723d7768697465)

## Descrição

Este projeto é uma API desenvolvida com **Java, Java Spring, Flyway Migrations e HSQLDB** como banco de dados. O objetivo foi criar um painel de gerenciamento de eventos presenciais, um desafio proposto durante a [Next Level Week Unite](https://www.rocketseat.com.br/eventos/nlw?utm_source=kipperdev&utm_medium=organic&utm_campaign=lead&utm_term=evento-nlw&utm_content=pagevento-lp_evento_nlw_unite_inscricao), um evento gratuito onde tive a oportunidade de desenvolver o projeto do zero vendo às vídeo aulas da [Fernanda Kipper](https://github.com/Fernanda-Kipper)

Durante o desenvolvimento deste projeto, aprendi a integrar diversas tecnologias e a construir uma API funcional com Java e Spring, além de aplicar boas práticas de versionamento e migração de banco de dados com Flyway. Foi um processo enriquecedor e desafiador, e fico feliz em vê-lo concluído.

## Requisitos

### Requisitos Funcionais

-   O organizador deve ser capaz de registrar um novo evento.
-   O organizador deve ser capaz de visualizar os dados do evento.
-   O organizador deve ser capaz de visualizar a lista de participantes.
-   O participante deve ser capaz de se inscrever em um evento.
-   O participante deve ser capaz de visualizar seu crachá de inscrição.
-   O participante deve ser capaz de fazer check-in no evento.

### Regras de Negócio

-   Participantes só podem se inscrever em um evento uma vez.
-   Participantes só podem se inscrever em eventos com vagas disponíveis.
-   Participantes só podem fazer check-in em um evento uma vez.

### Requisitos Não Funcionais

-   O check-in no evento será realizado usando um QRCode.

## Instalação

1.  Clone o repositório:

    `git clone https://github.com/usuario/repositorio.git` 
    
2.  Instale as dependências com Maven
    

## Uso

1.  Inicie a aplicação com Maven
2.  A API estará acessível em [http://localhost:8080](http://localhost:8080/)
    

## Endpoints da API

A API fornece os seguintes endpoints:

-   **POST /events** - Registra um novo evento.
-   **GET /events/{eventId}** - Recupera os detalhes de um evento.
-   **GET /events/attendees/{eventId}** - Recupera a lista de participantes registrados para o evento especificado.
-   **POST /events/{eventId}/attendees** - Registra um novo participante no evento.
-   **POST /attendees/{attendeeId}/badge** - Recupera o crachá do participante para acessar o evento.
-   **POST /attendees/{attendeeId}/check-in** - Realiza o check-in do participante no evento.

----------

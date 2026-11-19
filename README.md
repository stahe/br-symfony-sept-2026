# Introdução passo a passo ao framework web [Symfony]

**O curso está disponível online aqui: [https://stahe.github.io/br-symfony-sept-2026/](https://stahe.github.io/br-symfony-sept-2026/)**

## Autor

O curso e todo o seu código foram escritos por **Claude**, a IA da Anthropic, o **único autor**, a pedido de Serge Tahé (setembro de 2026).

## Visão geral

Este curso apresenta um guia passo a passo para construir uma aplicação web MVC usando o framework **Symfony 8.1** e a linguagem **PHP 8.4**. As páginas HTML são geradas pelo servidor por meio de views **Twig**, sem framework JavaScript no cliente. O acesso a dados é feito por meio do ORM **Doctrine**.

Ele adapta o curso [Introdução passo a passo ao framework web [Laravel](https://stahe.github.io/br-laravel-sept-2026/)]—que por sua vez se baseia nos cursos [Flask](https://stahe.github.io/br-flask-sept-2026/)— [Spring MVC](https://stahe.github.io/br-springmvc-sept-2026/), [ASP.NET Core MVC](https://stahe.github.io/br-aspnetcoremvc-sept-2026/) e [NestJS](https://stahe.github.io/br-nestjs-html-sept-2026/). Os exemplos têm os mesmos números e abordam os mesmos tópicos: você pode comparar os frameworks exemplo por exemplo.

## Conteúdo

| Capítulo | Tópicos | Exemplos |
|---|---|---|
| Actions, roteamento, respostas | rotas (`#[Route]`), controllers, respostas, redirecionamentos, contêiner de serviços | 01 a 06 |
| O modelo da action | parâmetros da requisição, argument resolvers, restrições de validação, requisições POST | 07–12 |
| A view e seu modelo | Twig, templates, macros, extensões, componente Form, validação, Post/Redirect/Get, proteção CSRF | 13–21 |
| Internacionalização | uma aplicação em francês e inglês (dicionários YAML, mensagens ICU) | 22 |
| Escopos de dados | requisição, sessão, cache, cookies | 23 |
| O ciclo de vida da requisição | eventos do núcleo, listeners, argument resolvers, páginas de erro | 24 |
| Autenticação e autorização | firewall, autenticador JWT em um cookie, papéis, CAPTCHA, limitação de taxa | 25–27 |
| Arquitetura em camadas | web / lógica de negócio / DAO com Doctrine e MySQL | 28 |
| Estudo de caso | **RdvMedecins**, uma aplicação de agendamento de consultas médicas, explicada arquivo por arquivo | - |

O estudo de caso `rdvmedecins2-symfony` gerencia três papéis (administrador, médicos, pacientes): agendas, reservas, gerenciamento de médicos e clientes, criação de conta protegida por CAPTCHA e uma interface em francês/inglês. Ele usa o mesmo banco de dados `dbrdvmedecins2` que as outras versões da aplicação.

## Pré-requisitos

- PHP 8.4 ou superior (extensões `intl`, `mbstring`, `openssl`, `pdo_mysql`);
- Composer 2;
- MySQL 8 ou MariaDB (Laragon no Windows);
- Visual Studio Code com as extensões PHP Intelephense, Twig Language 2 e YAML;
- curl.

O código-fonte pode ser baixado do site do curso. As pastas `vendor` não estão incluídas: `composer install` as cria—uma na pasta `exemples` e outra na pasta `rdvmedecins2-symfony`.

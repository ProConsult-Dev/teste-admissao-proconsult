# Teste admissional ProConsult

## Avisos antes de começar

- Crie um repositório no seu github.
- Faça seus commits no seu repositório.
- Envie apenas o link do repositório no formulário.

## Observação sobre o ambiente da aplicação

Use a versão do PHP até a 7.3.x.

Isso não quer dizer que você terá que mudar a versão do php da sua máquina, porém leve em consideração que funções e comportamentos introduzidos em versões superiores à 7.3.x não serão relevantes no dia a dia da empresa.

## Objetivo: Sistema de suporte

A aplicação que você deverá criar consiste num sistema de suporte fornecido por uma empresa aos seus clientes.

Para a empresa conseguir dar assistência, os clientes devem abrir um chamado na plataforma que será desenvolvida. Após a abertura do chamado, um colaborador da empresa poderá responder.

Requisitos:

- Fluxo de autenticação (cadastro e login apenas).

- Devem existir dois tipos de usuários: Cliente e Colaborador.

- Ambos os tipos de usuário precisarão de nome completo, CPF, e-mail e senha. CPF e e-mail devem ser únicos no sistema, ou seja, o sistema deve permitir apenas um cadastro com o mesmo CPF ou e-mail.

- Apenas usuários do tipo Cliente devem conseguir abrir chamados.

- Um chamado deve possuir título, descrição e anexos (opcional).

- Os chamados devem possuir 3 possíveis status: Aberto, Em atendimento e Finalizado. Um chamado deve nascer com o status Aberto. Quando um colaborador responder o chamado, ele deve passar para Em atendimento. Quando o chamado for finalizado, independente do problema ter sido resolvido ou não, deve ir para o status de Finalizado.

- Apenas usuários do tipo Colaborador devem conseguir responder os chamados abertos.

- Considere o funcionamento de um tópico de um fórum como exemplo para criar o ciclo de vida de um chamado, ou seja, desde sua abertura até sua finalização.

**Obs:** Caso não goste da proposta, você pode mudar o tema, porém é importante que a sua aplicação tenha os mesmos princípios da proposta do teste.

## Avaliação

Atente-se a cumprir a maioria dos requisitos, pois podem faltar alguns e durante a avaliação conversaremos a respeito do que faltou.

A avaliação levará em conta os seguintes critérios:

- Funcionalidade.
- Estrutura e organização do projeto.
- Tratamento de erros.
- Aspectos de segurança.
- Versionamento do código.

## O que **não** será avaliado

- Design da parte front-end da aplicação.

## Diferencial

- Rest.
- Testes.
- Documentação.
- Uso de um framework.

## Observações finais

A aplicação não precisa ser complexa. Você pode desenvolver separando o back-end do front-end, utilizando o Laravel com o VueJs, quanto fazendo somente um módulo, como nas aplicações mais antigas.

A autenticação não precisa ser complexa. Pode ser feita também sem o auxílio de um framework por meio de sessões ou com algum pacote que já implementa essas funcionalidades, como por exemplo o Sanctum, utilizando tokens ou cookie.

Caso não utilize um banco de dados convencional como o MySQL ou Postgresql, coloque no readme do seu repositório as instruções de setup do ambiente para agilizar o processo. Caso queira usar docker também será permitido, porém não é algo que será avaliado.
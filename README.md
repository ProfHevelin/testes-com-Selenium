# Teste Automatizado de Cadastro com Selenium WebDriver

Esta documentação apresenta como executar um teste automatizado de Front-End para verificar o **cadastro de produtos** na aplicação Angular CRUD API.

**Projeto utilizado:** [Angular CRUD API — GitHub](https://github.com/ProfHevelin/angular-crud-api)

O teste utiliza o **Selenium WebDriver com Node.js** para simular as ações de um usuário no navegador, como acessar a página de cadastro, preencher os campos do formulário e clicar no botão para cadastrar um produto.

## 1. Objetivo do teste

O objetivo é verificar se o formulário de cadastro de produtos funciona conforme o esperado, observando se a aplicação permite preencher os campos e concluir o cadastro.

Durante o teste, serão verificadas as seguintes etapas:

* Abertura da página de cadastro de produtos.
* Preenchimento dos campos do formulário.
* Acionamento do botão de cadastro.
* Verificação do resultado apresentado pela aplicação.

## 2. Pré-requisitos

Antes de executar o teste, verifique se você possui:

* Node.js instalado.
* Google Chrome instalado.
* Projeto Angular CRUD API configurado e em execução.
* Selenium WebDriver instalado na pasta do projeto de testes.

A aplicação Front-End deve estar acessível localmente, por exemplo:

`http://localhost:4200`

## 3. Preparação do ambiente

Caso o ambiente ainda não esteja configurado, siga estas etapas:

**1. Crie uma pasta para os testes**, por exemplo:

`testes-selenium`

**2. Abra o terminal nessa pasta** e inicialize o projeto Node.js:

```bash
npm init -y
```

**3. Instale o Selenium WebDriver:**

```bash
npm install selenium-webdriver
```

Esses procedimentos precisam ser realizados apenas na configuração inicial do ambiente ou quando for necessário reinstalar as dependências.

## 4. Executar a aplicação

Antes de iniciar o teste automatizado, é necessário executar a aplicação Angular CRUD API.

As instruções para configurar e executar a aplicação estão disponíveis no próprio repositório do projeto no GitHub:

[Angular CRUD API — Repositório do projeto](https://github.com/ProfHevelin/angular-crud-api)

Consulte as orientações descritas no repositório e siga os procedimentos necessários para iniciar a aplicação.

Após a inicialização, confirme se o Front-End está funcionando corretamente no navegador e mantenha a aplicação em execução durante todo o teste automatizado.


## 5. Executar o teste automatizado

Com o ambiente configurado e a aplicação em execução, abra um terminal na pasta onde está localizado o arquivo de teste.

Para executar o teste de cadastro, utilize:

```bash
node cadastro-produto.test.js
```

**Importante:** para executar o teste, basta informar `node` seguido do nome do arquivo `.js`. Não é necessário executar novamente `npm init -y` ou instalar o Selenium a cada execução.

O nome do arquivo utilizado no comando deve corresponder exatamente ao arquivo de teste existente na pasta.

## 6. Resultado esperado

Durante a execução, o Selenium deverá automatizar as ações previstas no script, como:

1. Abrir o Google Chrome.
2. Acessar a página de cadastro de produtos.
3. Preencher os campos do formulário.
4. Clicar no botão de cadastro.
5. Verificar o resultado do cadastro, conforme as validações implementadas no teste.

Ao final, observe se o produto foi cadastrado corretamente e se a aplicação apresentou a mensagem ou o comportamento esperado.

## 7. Conclusão

O Selenium WebDriver permite automatizar interações com a interface da aplicação, reduzindo a necessidade de repetir manualmente os mesmos passos.

Neste exemplo, o foco é o **teste automatizado do cadastro de produtos do projeto Angular CRUD API**. O resultado deve ser avaliado considerando não apenas a execução das ações no navegador, mas também a confirmação de que o cadastro ocorreu corretamente.

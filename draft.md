# AngularJS App usando Yeoman

## Apresentação
Meu apresento

## O que vamos ver

* Yeoman e Generators
* Bower
* Grunt
* AngularJS
	* Gerando o App
	* Instalando uma nova dependencia (bower)
	* Yeoman Generators
	* Tests

## Pré-requisitos

* Você precisa ter conhecimentos básicos de linha de comando
* Ter o [NodeJS e NPM](http://nodejs.org/) instalados
* Bons conhecimentos em Javascript, CSS e HTML

## Yeoman e Generators

O Yeoman vai além de uma ferramenta, é um workflow. 

Conjunto de ferramentas e boas praticas fazendo que o desenvolvimento para web melhor e mais ágil.

Foco em aumentar a produtividade.

### Instalação:

	npm install -g yo

Essa instrução já vai instalar o Yeoman, Grunt e Bower automaticamente.

### Ferramentas:

* yo, scaffolding tool
* grunt, tasks tool
* bower, package mandagement

#### Yo

Inicializa o seu projeto, criando o esqueleto da aplicação, criar uma configuração para o ```bower``` e para o ```grunt``` já implementando algumas tasks essenciais que você provavelmente vai precisar.

#### Grunt

Automatiza tarefas repetitivas, como fazer build, testes e preparar o projeto para ser executado.

#### Bower 

Gerência as dependências do seu projeto, você não precisa mais ficar fazendo download manual e gerenciar versões de bibliotecas de terceiros.

#### Yeoman Generators

São como receitas para você inicializar seu projeto. 

A idéia por trás desse conceito é você criar os esqueletos dos seus projetos com as suas boas práticas e conveções.

Já existe uma série de Generators disponíveis. Você pode encontrar executando essa instrução no seu terminal.

	npm search yeoman-generator

Nós vamos usar o generator no AngularJS:

	npm install -g generator-angular

## Bower

## Grunt

Para aumentar a velocidade do Desenvolvimento automatizando tarefas repetitivas

## AngularJS

É um framework com uma série de peculiaridades e características eficientes e poderosas.

### Gerando um app AngularJS com Yeoman

Para gerar o App você só precisa disso:

	yo angular

O Generator vai fazer uma série de perguntas do que você pretende instalar. Você pode responder sim para Twitter`s Bootstrap e sim para inclur ngResource. O resto não vamos precisar nesse caso.

Em alguns segundos o generator faz a magica dele e temos uma aplicação funcionando. O Yeoman vai criar vários arquivos e pastas, executa o ```bower install``` (para instalar as dependências da aplicação) e executa o ```npm install``` (para instalar as dependências das tarefas do grunt).

Algmas pastas e arquivos importante:

**app/: ** A pasta contém os seus arquivos estáticos, seu html, css e javascript, onde provavelmente você vai passar a maior parte do seu tempo. 

**package.json: ** Esse arquivo configura o que o npm fará no seu projeto. Ele gerência as depêndencias das tarefas do grunt.

**node_modules/: ** A pasta onde o npm instala suas dependências.

**Gruntfile.js :** É um arquivo javascript responsavel por configurar as tarefas que o grunt vai executar no seu projeto. Ele define variáveis de ambiente, as tarefas e a sequência que as tarefas serão executadas.

**bower.json: ** Ele funciona como o ```package.json```, mas para o bower. Em algumas versões mais antigas esse arquivo pode ser component.json.

**.bowerrc: ** Ele configura algumas variáveis gerais do bower.

**arquivos Karma: ** Karma é um framework de testes. Esses arquivos configuram ou executam alguns testes na sua aplicação.

Esse são alguns arquivos que eu defini como importante, mas existem muito outros, cada um com uma funcionalidade e foco durante o workflow.

### Instalando uma nova dependencia (bower)

### Yeoman Generators

### Tests

### Build

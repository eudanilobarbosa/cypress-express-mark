# Cypress@12.2.0 + Mark L - Gerenciador de Tarefas

Repositório do projeto de testes End-to-end (E2E) feitos com **Cypress** :green_heart: para o web app de demonstração: *Mark L - Gerenciador de Tarefas*.

___

## IDE utilizada nesse projeto

[VS Code](https://code.visualstudio.com/) versão `1.88.1`
   - Extensões
     - [One Dark Pro (Darker)](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme)
     - [Material Icon Theme](https://marketplace.visualstudio.com/items?itemName=PKief.material-icon-theme)
     - [Cucumber (Gherkin) Full Support](https://marketplace.visualstudio.com/items?itemName=alexkrechik.cucumberautocomplete)
     - [SQLite Viewer](https://marketplace.visualstudio.com/items?itemName=qwtel.sqlite-viewer)

## Pré-requisitos

Você vai precisar dos seguintes sistemas instalados em seu computador:
- [Windows Terminal](https://apps.microsoft.com/detail/9n0dx20hk701?hl=pt-br&gl=BR)
- [Node.js](https://nodejs.org/dist/v18.12.1/node-v18.12.1-x64.msi) versão `v18.12.1`
  - NPM versão `8.19.2`
- [Git](https://github.com/git-for-windows/git/releases/download/v2.43.0.windows.1/Git-2.43.0-64-bit.exe) versão `2.43.0.windows.1`

> [!NOTE]
> Durante a instalação do Node.js o NPM é automaticamente instalado.

> [!IMPORTANT]
> Para a instalação do Git garantir que as opções "Git Bash Here" e "(NEW!) Add a Git Bash Profile to Windows Terminal" estejam marcadas :white_check_mark:.

## Instalação

### Clonar o repositório

1. Instalar as dependências da web app que estão na pasta **/apps/markL/**, pasta **api** - Api do gerenciador de tarefas, execute o comando
```
npm i
```

2. Para inicializar e criar o banco de dados SQLite da Api, execute o comando
```
npm run db:init
```

3. Colocar Api em execução
```
npm run dev
```

4. Pasta **web** - Interface gráfica do gerenciador de tarefas, execute o comando
```
npm i
```

5. Colocar Interface gráfica em execução
```
npm run dev
```

## Como executar

1. Instalar as dependências da web app que estão na pasta **/apps/markL/**, pasta **api** - Api do gerenciador de tarefas, execute o comando
```
npm i
```

2. Para inicializar e criar o banco de dados SQLite da Api, execute o comando
```
npm run db:init
```

3. Pasta **web** - Interface gráfica do gerenciador de tarefas, execute o comando
```
npm i
```

## Testes

Este projeto utiliza o [Cypress.io](https://cypress.io) para os testes _end-to-end_, onde você pode executá-los tanto em modo interativo, como em modo _headless_.

1. Instalar as dependências do Cypress que estão na pasta raiz **/**, execute o comando `npm i`

Além disso, as execuções dos testes são gravadas no servidor local [Allure Report](https://allurereport.org/).

### Modo _headless_

Execute `npx cypress run` para rodar todos os testes em modo _headless_.

> [!TIP]
> Execute os testes através do Lauchpad, modo interativo do Cypress, execute o comando `npx cypress open`

# Funcionalidades Testadas

## home

* [x] webapp deve estar online

## tarefas
### cadastro

* [x] deve cadastrar uma nova tarefa
* [x] não deve permitir tarefa duplicada
* [x] campo obrigatório

### atualização

* [x] deve concluir uma tarefa

### exclusão

* [x] deve remover uma tarefa

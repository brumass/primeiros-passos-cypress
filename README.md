# Testes Automatizados com Cypress - OrangeHRM

Este projeto contém testes automatizados utilizando o framework [Cypress](https://www.cypress.io/) para validação do login no sistema **[OrangeHRM Demo](https://opensource-demo.orangehrmlive.com/)**.

## Estrutura dos Testes

O arquivo de testes `login.cy.js` inclui dois cenários principais:

### ✅ Cenário: Login com Sucesso
- Dado que o usuário acessa a página de login do OrangeHRM
- Quando o usuário informa o nome de usuário "Admin"
- E  informa a senha "admin123"
- E  clica no botão de login
- Então o sistema deve redirecionar para a página "/web/index.php/dashboard/index"
- E deve exibir o título "Dashboard" na tela

### ❌ Cenário: Login com Falha
- Dado que o usuário acessa a página de login do OrangeHRM
- Quando o usuário informa o nome de usuário "teste"
- E informa a senha "teste"
- E clica no botão de login
- Então o sistema deve exibir uma mensagem "Invalid credentials"
  
## Pré-requisitos

- [Node.js](https://nodejs.org/) instalado
- [Cypress](https://docs.cypress.io/guides/getting-started/installing-cypress) instalado no projeto:

 npm install cypress --save-dev

🧑‍💻 Projeto desenvolvido para fins de estudo com automação de testes em aplicações web usando Cypress.

```bash

## Como Executar os Testes

###Clone o repositório:

git clone https://github.com/brumass/primeiros-passos-cypress.git
cd primeiros-passos-cypress.git

###Abra o Cypress:

npx cypress open
Na interface do Cypress, clique no arquivo login.cy.js para executar os testes.




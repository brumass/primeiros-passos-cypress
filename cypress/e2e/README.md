# Testes Automatizados com Cypress - OrangeHRM

Este projeto contém testes automatizados utilizando o framework [Cypress](https://www.cypress.io/) para validação do login no sistema **[OrangeHRM Demo](https://opensource-demo.orangehrmlive.com/)**.

## Estrutura dos Testes

O arquivo de testes `login.cy.js` inclui dois cenários principais:

### ✅ Login com Sucesso
- Acessa a página de login do OrangeHRM.
- Insere as credenciais válidas:  
  - **Usuário:** Admin  
  - **Senha:** admin123
- Verifica o redirecionamento para o painel principal (`/dashboard/index`).
- Confirma que o título **Dashboard** está visível na tela.

### ❌ Login com Falha
- Acessa a página de login do OrangeHRM.
- Insere credenciais inválidas.
- Verifica que uma mensagem de erro (alerta) é exibida.

## Pré-requisitos

- [Node.js](https://nodejs.org/) instalado
- [Cypress](https://docs.cypress.io/guides/getting-started/installing-cypress) instalado no projeto:

```bash
npm install cypress --save-dev


## Como Executar os Testes

*Clone o repositório:*

git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

*Abra o Cypress:*

npx cypress open
Na interface do Cypress, clique no arquivo orangehrm.cy.js para executar os testes.

🧑‍💻 Autor
Projeto desenvolvido para fins de estudo com automação de testes em aplicações web usando Cypress.


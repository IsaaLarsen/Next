# Sistema de Cadastro de Profissões - Frontend

Este é o frontend do sistema de cadastro de profissões, desenvolvido utilizando Next.js, responsável por fornecer a interface de cadastro e enviar os dados para o backend.

## Configuração do Projeto

### Pré-requisitos:
- Node.js 16.0 ou superior
- npm ou yarn

### Passos para Configuração:
1. Clone este repositório:
   git clone https://github.com/Isaalarsen/next.git

2. Acesse o diretório do projeto:
   cd nextjs-frontend

3. Instale as dependências do projeto:
   Com npm:
   npm install
   Ou com yarn:
   yarn install

4. Inicie o servidor de desenvolvimento:
   npm run dev
   Ou com yarn:
   yarn dev
   O frontend estará disponível em http://localhost:3000/cadastro.

## Funcionalidade Implementada

### Cadastro de Profissões
- O frontend possui um formulário que permite o cadastro de uma nova profissão.
- O formulário coleta os seguintes dados:
  - Nome da profissão (obrigatório)
  - Descrição da profissão (opcional)
  - Salário (obrigatório)
  - Empresa associada (obrigatório)

### Fluxo de Dados:
1. O usuário preenche o formulário com as informações da profissão.
2. Quando o formulário é enviado, os dados são validados no frontend:
   - O campo "salário" só aceita números e deve ter pelo menos 2 dígitos.
   - Nenhum campo pode ficar em branco.
   - O campo "salário" não pode ser vazio e deve ser um valor numérico válido.
3. Após validação, o frontend envia os dados para o backend através de uma requisição POST para `http://127.0.0.1:8000/api/profissoes`.
4. O backend processa os dados e retorna uma resposta indicando se o cadastro foi realizado com sucesso ou se ocorreu um erro.

## Estrutura de Componentes

O projeto é composto por:
- **Formulário de Cadastro**: Com os campos Nome, Descrição, Salário e Empresa.
- **Validação de Formulário**: O frontend valida os dados antes de enviar para o backend.
- **Integração com API**: O formulário envia os dados para a API do backend utilizando o método POST.

## Estrutura de Pastas

/pages /index.tsx 

# Página principal com o formulário 
/styles /cadastro.module.css 

# Estilos específicos do formulário 
/components /Cadastro.tsx 

# Componente de cadastro de profissões 
/public /favicon.ico 


## Contribuidores

- Isadora Larsen - GitHub: https://github.com/IsaaLarsen

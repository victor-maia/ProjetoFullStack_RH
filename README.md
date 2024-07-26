# Gerenciamento de Funcionários - Fullstack 📋👨‍💼👩‍💼

Este projeto consiste em uma aplicação para o gerenciamento de informações de funcionários, com backend desenvolvido em .NET e frontend em Angular. O sistema oferece funcionalidades para criar, visualizar, atualizar, inativar e excluir registros de funcionários.

## Funcionalidades Principais 🛠️

### 1. Visualizar Funcionários 📜
   - Exibe uma lista de todos os funcionários registrados na base de dados.
   - Rota: `/funcionarios`

### 2. Detalhes do Funcionário 🔍
   - Exibe os detalhes de um funcionário específico com base no ID fornecido.
   - Rota: `/funcionarios/{id}`

### 3. Cadastrar Novo Funcionário 📝
   - Permite criar um novo registro de funcionário com os dados fornecidos.
   - Rota: `/cadastro`

### 4. Editar Funcionário ✏️
   - Permite atualizar os detalhes de um funcionário existente.
   - Rota: `/editar/{id}`

### 5. Inativar Funcionário 🚫
   - Permite inativar o registro de um funcionário na sessão de detalhes.
   - Rota: `/funcionarios/inativar/{id}`

### 6. Excluir Funcionário 🗑️
   - Permite excluir o registro de um funcionário.
   - Rota: `/funcionarios/excluir/{id}`


## Endpoints 🚀

### 1. GetFuncionarios
**Método:** `GET`  
**Rota:** `/api/funcionario`  
**Descrição:** Retorna uma lista de todos os funcionários registrados na base de dados. 📜

### 2. GetFuncionarioById
**Método:** `GET`  
**Rota:** `/api/funcionario/{id}`  
**Descrição:** Retorna os detalhes de um funcionário específico com base no ID fornecido. 🔍

### 3. CreateFuncionarios
**Método:** `POST`  
**Rota:** `/api/funcionario`  
**Descrição:** Cria um novo registro de funcionário com os dados fornecidos no corpo da requisição. ✍️

### 4. InativaFuncionario
**Método:** `PUT`  
**Rota:** `/api/funcionario/{id}`  
**Descrição:** Inativa o registro de um funcionário específico com base no ID fornecido. 🚫

### 5. UpdateFuncionario
**Método:** `PUT`  
**Rota:** `/api/funcionario`  
**Descrição:** Atualiza os detalhes de um funcionário com os dados fornecidos no corpo da requisição. 🔄

### 6. DeleteFuncionario
**Método:** `DELETE`  
**Rota:** `/api/funcionario/{id}`  
**Descrição:** Exclui o registro de um funcionário específico com base no ID fornecido. 🗑️

## Modelos de Dados 📊

### FuncionarioModel
- `Id`: Número de identificação do funcionário. 🆔
- `Nome`: Nome do funcionário. 🏷️
- `DepartamentoEnum`: Departamento do funcionário, (Enum). 🏢
- `Ativo`: Status do funcionário (True/False). ✅/❌
- `TurnoEnum`: Turno do funcionário (Enum). ⏰
- `DataDeCriacao`: Data de criação do funcionário. 📅
- `DataDeAlteracao`: Data de alteração do funcionário. 📅

## Respostas de Serviço 💬

Todos os endpoints retornam uma resposta do serviço que inclui um status de sucesso/falha e os dados relevantes. 🟢🔴

## Requisitos 🛠️

- .NET 6 ou superior
- Entity Framework Core
- Angular CLI

## Contribuição 🤝

Contribuições são bem-vindas! Sinta-se à vontade para abrir um problema ou enviar um pull request. 🚀

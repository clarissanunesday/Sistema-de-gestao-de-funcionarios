# Sistema de Gestão de Funcionários

Este projeto é um sistema de gerenciamento de funcionários que permite o cadastro de funcionários, departamentos e seus salários. O sistema oferece funcionalidades para registrar, consultar e manipular informações sobre funcionários e departamentos.

## Funcionalidades

- **Gestão de Funcionários**: Cadastro de funcionários com informações como nome, cargo, salário e departamento.
- **Gestão de Departamentos**: Registro de departamentos e a relação com os funcionários.
- **Gestão de Salários**: Registro de salários para cada funcionário, permitindo o controle histórico.
- **Consultas Avançadas**: Consultas para visualizar a lista de funcionários, salários totais por departamento e históricos de salários.

## Estrutura do Banco de Dados

### Tabelas

- **Departamentos**:
  - `id_departamento`: Identificador único do departamento.
  - `nome`: Nome do departamento.

- **Funcionarios**:
  - `id_funcionario`: Identificador único do funcionário.
  - `nome`: Nome completo do funcionário.
  - `cargo`: Cargo do funcionário na empresa.
  - `salario`: Salário do funcionário.
  - `id_departamento`: Referência ao departamento do funcionário.

- **Salarios**:
  - `id_salario`: Identificador único do registro de salário.
  - `id_funcionario`: Referência ao funcionário correspondente.
  - `data`: Data do registro salarial.
  - `valor`: Valor do salário.

## Consultas e Operações Disponíveis

### Consultas

1. **Listar todos os funcionários e seus respectivos departamentos**:
   - Exibe todos os funcionários registrados com seus respectivos cargos, salários e departamentos.

2. **Mostrar o salário total de cada departamento**:
   - Exibe o total de salários pagos por cada departamento.

3. **Verificar os salários históricos de um funcionário específico**:
   - Exibe todos os registros de salários de um funcionário específico.

### Atualizações e Deleções

1. **Atualizar o nome do departamento**:
   - Permite atualizar o nome de um departamento existente.

2. **Atualizar o salário de um funcionário específico**:
   - Permite atualizar o salário de um funcionário usando sua chave primária.

3. **Remover um funcionário e seus registros de salários**:
   - Permite excluir um funcionário e todos os registros de salários associados.

4. **Remover um departamento**:
   - Permite excluir um departamento, desde que não haja funcionários associados a ele.

## Como Usar

1. **Criar o Banco de Dados**:
   Execute o script SQL fornecido para criar o banco de dados e suas respectivas tabelas.

2. **Inserir Dados**:
   Insira dados de departamentos, funcionários e salários conforme necessário.

3. **Consultar e Manipular Dados**:
   Utilize as consultas SQL fornecidas para visualizar e modificar os dados.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## Requisitos

- MySQL ou outro sistema de gerenciamento de banco de dados compatível com SQL.
- Ferramenta para execução de scripts SQL, como MySQL Workbench ou phpMyAdmin.

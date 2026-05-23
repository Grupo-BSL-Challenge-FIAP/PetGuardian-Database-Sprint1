# Projeto Database: Clyvo Vet

Este repositório contém o script completo de modelagem, estruturação e lógica procedimental (PL/SQL) desenvolvido para o Challenge 2026 – *Mastering Relational and Non-Relational Database*.

## 📋 Descrição do Projeto
O **Clyvo Vet** é um ecossistema de gestão clínica veterinária focado na monitorização da saúde e bem-estar animal. O banco de dados foi desenhado para garantir integridade, segurança nas operações e inteligência na extração de dados clínicos.

## 👩🏾‍🦱🧑🏾👧🏻 Integrantes
* Manuela de Lacerda Soares - RM 564887 
* Moisés Barsoti Andrade de Oliveira - RM 565049 
* Sofia Siqueira Fontes - RM 563829      

## 🛠 Funcionalidades Implementadas
* **Modelagem Relacional (3FN):** Estrutura normalizada que cobre clientes, pets, veterinários, históricos clínicos e agendamentos.
* **Procedimentos de Carga (Procedures):** Camada de abstração que protege as tabelas contra inserções diretas, contendo validações de regra de negócio e tratamento de erros.
* **Auditoria Automática:** Tabela de `T_LOG_ERROS_PG` que captura violações de integridade e falhas de runtime, garantindo rastreabilidade.
* **Inteligência de Negócio (Relatórios):** Blocos PL/SQL que realizam análises de risco, triagem de pacientes e métricas de saúde com uso de funções analíticas (`LAG`, `LEAD`) e cursores explícitos.

## 🗄 Estrutura do Script
1. **Limpeza:** Remoção de objetos existentes (DROP).
2. **DDL:** Criação das tabelas e definições de chaves (`PK`, `FK`, `CHECK`).
3. **Procedures:** Definição das rotinas de inserção com tratamento de exceções.
4. **Carga (DML):** Execução das chamadas às procedures para popular o banco.
5. **Análise:** Blocos PL/SQL para gerar os relatórios de gestão.

## 🚀 Como Executar
1. Utiliza o **Oracle SQL Developer** ou a tua ferramenta preferida de gestão de base de dados Oracle.
2. Cria um novo script SQL e cola o conteúdo do ficheiro de script.
3. Executa o script completo pressionando **F5** (Run Script) para que a ordem de criação, populamento e análise seja respeitada.

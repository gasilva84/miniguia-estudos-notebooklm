# Miniguia de Estudos: SAP PowerDesigner com NotebookLM

Este repositório documenta a utilização do **NotebookLM** da Google como ferramenta de aprendizagem da ferramenta **SAP PowerDesigner**.

---

## 1. Contexto e Objetivos

* **Tema Escolhido:** SAP PowerDesigner — Modelagem de Dados.
* **Objetivos de Estudo:**
  1. Compreender a transição entre o Modelo Conceitual de Dados (CDM), Lógico (LDM) e Físico (PDM).
  2. Aprender a definir estruturas de bancos de dados (tabelas, colunas, chaves e restrições).
  3. Explorar o uso de IA na síntese de documentações técnicas complexas através de engenharia de prompts.

---

## 2. Curadoria de Fontes

Foram selecionadas 3 fontes oficiais e técnicas para alimentar o caderno no NotebookLM:

1. **SAP Help Portal:** Quick Reference para Physical Data Model (PDM).
2. **SAP PowerDesigner Data Modeling Guide:** Documentação técnica completa em PDF cobrindo CDM, LDM e PDM.
3. **SAP PowerDesigner Overview:** Apresentação técnica sobre repositório e arquitetura de metadados.

---

## 3. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

* **Desafio Encontrado:** Ao utilizar prompts curtos e genéricos, a IA fornecia explicações genéricas da web sobre modelagem.
* **Solução e Refinamento:** Adicionar restrições de contexto baseadas nas fontes permitiu obter respostas estruturadas sobre comandos específicos, tais como o uso do *Generation Options* e configuração de integridade referencial no PDM.

---

## 4. Miniguia de Estudo (Entrega Final)

### 📌 Resumos Estruturados
* **A Ferramenta:** O SAP PowerDesigner é uma solução corporativa para gerenciamento de metadados e modelagem de arquitetura de dados/negócios.
* **Camadas de Modelagem:**
  * **CDM (Modelo Conceitual):** Mapeia entidades e relacionamentos sob a ótica do negócio.
  * **LDM (Modelo Lógico):** Refina atributos e aplica normalização sem dependência de SGBD.
  * **PDM (Modelo Físico):** Converte a estrutura lógica para o SGBD alvo, gerando comandos DDL, tabelas, chaves primárias/estrangeiras e restrições (*constraints*).

### 📖 Glossário de Conceitos
* **Repositório Central:** Banco de dados unificado para versionamento de modelos em equipe (*Check-in / Check-out*).
* **Engenharia Reversa:** Capacidade de ler um banco de dados relacional existente e gerar seu PDM correspondente.
* **Constraints (Restrições):** Regras de validação de dados aplicadas no PDM (como *Check Constraints* e *Foreign Keys*).

### 🛠️ Prompts Reutilizáveis para Revisão
1. *"Resuma as diferenças de mapeamento entre tipos de dados conceituais e tipos físicos por SGBD segundo o manual."*
2. *"Explique como o PowerDesigner lida com a geração automática de chaves estrangeiras na transição de CDM para PDM."*
3. *"Quais as boas práticas para evitar conflitos ao salvar alterações no Repositório do PowerDesigner?"*

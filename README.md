# 🧠 Sistema Especialista de Triagem de Alertas

Este projeto implementa um **Sistema Especialista baseado em regras de produção**, utilizando **CLIPS integrado ao Python via clipspy**, com o objetivo de diagnosticar automaticamente incidentes em infraestrutura de TI a partir de alertas e métricas.

---

## 🎯 Objetivo

Receber alertas de infraestrutura (logs, métricas e estados do sistema) e inferir automaticamente:

- Diagnóstico do problema
- Prioridade do incidente
- Ação recomendada
- Equipe responsável
- Supressão de alertas secundários
- Justificativa da decisão
- Trilha de regras acionadas

---

## 🧠 Conceitos de IA Utilizados

- Sistemas Especialistas
- Regras de Produção (IF-THEN)
- Encadeamento para frente (Forward Chaining)
- Motor de Inferência (CLIPS)
- Base de Conhecimento
- Explicabilidade (Explainable AI)

---

## 🏗️ Arquitetura

A solução segue a separação clássica de sistemas especialistas:

### 🔹 Python
Responsável por:
- Leitura do JSON de entrada
- Transformação em fatos
- Execução do motor de inferência
- Coleta e formatação dos resultados

### 🔹 CLIPS (via clipspy)
Responsável por:
- Definição de fatos (templates)
- Regras de inferência
- Priorização de regras (`salience`)
- Tomada de decisão

---

## 📦 Estrutura (versão single-file)

# aml_agent_case
Agente de IA AML

# AML Agent Case

## 1. Visão Geral

Este projeto é um complemento ao [AML-FT Case](https://github.com/gabriel-cds/aml_case), focado na automação, padronização e apoio à decisão no processo de Prevenção à Lavagem de Dinheiro (AML) utilizando agentes de IA.

O objetivo é operacionalizar etapas críticas do pipeline AML, desde a ingestão e qualidade dos dados até a geração de relatórios SAR, integrando regras determinísticas, machine learning e automação.

> Consulte o projeto principal para contexto, dados e metodologia: [AML-FT Case](https://github.com/gabriel-cds/aml_case)

---

## 2. Arquitetura dos Agentes

O projeto está estruturado em quatro agentes principais:

- **Agent 1:** Ingestão e qualidade dos dados
- **Agent 2:** Feature Engineering
- **Agent 3:** ML Scoring
- **Agent 4:** SAR Report

Cada agente executa uma etapa específica do pipeline AML, permitindo modularidade, reuso e fácil manutenção.

<!-- Opcional: inserir diagrama de fluxo entre agentes -->

---

## 3. Estrutura do Projeto

```
├── agent.ipynb                # Notebook principal de execução dos agentes
├── artifacts/                 # Artefatos gerados por cada agente (planos, features, rankings, SAR)
├── features/                  # Scripts e dados de engenharia de features
├── models/                    # Modelos de machine learning e artefatos relacionados
├── raw/                       # Dados brutos
├── trusted/                   # Dados confiáveis e processados
```

---

## 4. Como Executar

### Pré-requisitos

- Python 3.10+
- Ambiente virtual (recomendado)
- Instalar dependências (requirements.txt ou pip freeze)

### Passos para execução

1. Clone o repositório e acesse a pasta do projeto:
	```bash
	git clone https://github.com/gabriel-cds/aml_agent_case.git
	cd aml_agent_case
	```
2. Crie e ative o ambiente virtual:
	```bash
	python -m venv venv
	# Windows:
	venv\Scripts\activate
	# Linux/Mac:
	source venv/bin/activate
	```
3. Instale as dependências:
	```bash
	pip install -r requirements.txt
	```
4. Execute o notebook principal.

---

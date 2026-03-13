
# AML Agent Case

## 1. Visão Geral

Este projeto é um complemento ao [AML-FT Case](https://github.com/gabriel-cds/aml_case), focado na automação, padronização e apoio à decisão no processo de Prevenção à Lavagem de Dinheiro (AML) utilizando agentes de IA.

O objetivo é operacionalizar etapas críticas do pipeline AML com o uso de IA, desde a ingestão e qualidade dos dados até a geração de relatórios SAR, ampliando escala, consistência e eficiência do processo de AML.

Consulte o projeto principal para contexto, dados e metodologia: [AML-FT Case](https://github.com/gabriel-cds/aml_case)

## 2. Arquitetura dos Agentes

O projeto está estruturado em quatro agentes principais:

- **Agent 1:** Ingestão e qualidade dos dados
- **Agent 2:** Feature Engineering
- **Agent 3:** ML Scoring
- **Agent 4:** SAR Report

Cada agente executa uma etapa específica do pipeline AML, permitindo modularidade, reuso e fácil manutenção.

## 3. Estrutura do Projeto

```
├── agent.ipynb                # Notebook principal de execução dos agentes
├── artifacts/                 # Artefatos gerados por cada agente (planos, features, rankings, SAR)
├── features/                  # Scripts e dados de engenharia de features
├── models/                    # Modelos de machine learning e artefatos relacionados
├── raw/                       # Dados brutos
├── trusted/                   # Dados confiáveis e processados
```
Observação: Apenas a pasta `raw` e o arquivo `agent.ipynb` existem inicialmente no repositório. As demais pastas (artifacts, features, models, trusted) são criadas automaticamente durante a execução do projeto.

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
4. Substitua a chave de API genérica no arquivo `.env` pela sua chave da OpenAI:
   - Abra o arquivo `.env` na raiz do projeto.
   - Localize a linha referente à chave da OpenAI (por exemplo, `OPENAI_API_KEY=...`).
   - Substitua pelo valor da sua chave pessoal.

5. Execute o notebook principal.

## Contato
<div> 
   <a href="https://www.linkedin.com/in/gabriel-candido-dos-santos-3793a6163" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
   <a href = "mailto:gabrielcandidosts@gmail.com"><img src="https://img.shields.io/badge/-Gmail-%23333?style=for-the-badge&logo=gmail&logoColor=white" target="_blank"></a>
</div>

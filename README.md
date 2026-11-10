# Automação Financeira — API de Processamento e Validação

Backend em **Python e FastAPI** para automatizar a leitura, organização e comparação de informações provenientes de diferentes relatórios financeiros.

## Problema e solução

A conferência manual de planilhas e arquivos com formatos distintos gera retrabalho e dificulta rastrear divergências. O projeto organiza um fluxo de **extração → consolidação → validação → relatório**, com regras específicas para cada tipo de documento.

## Funcionalidades presentes no repositório

- Extração e tratamento de arquivos identificados como **R189, QPE, SPB e NFSERV**.
- Consolidação de registros para permitir comparação entre fontes.
- Validações de dados e códigos utilizados na conferência.
- Geração de **relatórios de divergências**.
- Rotas de organização e processamento de arquivos.
- Módulos de integração com armazenamento e canais externos.

## Organização técnica

**Python · FastAPI · processamento de dados e arquivos · APIs REST**

- `app/api/routes/`: endpoints por tipo de operação.
- `app/core/extractors/`: extratores e normalização.
- `app/core/reports/`: relatórios comparativos e divergências.
- `app/core/services/`: orquestração do processamento.

**Interface web:** [Automação Financeira — Frontend](https://github.com/rodri-oliveira/automacao-financeira-web).  
**Versão desktop relacionada:** [Automação Financeira — Desktop](https://github.com/rodri-oliveira/automacao-financeira-desktop).

## Como avaliar

O ponto de entrada está em `app/main.py` e as dependências em `requirements.txt`. Há um script `run_server.py` para iniciar a API em desenvolvimento.

**Pré-requisitos para demonstração:** arquivos de exemplo compatíveis com os extratores e configuração dos serviços de integração. A execução integrada depende dessas fontes e dos serviços de apoio.

## Competências demonstradas

Automação com Python, APIs REST, modularização, regras de validação, tratamento de dados e geração de relatórios.

**Status:** implementação técnica documentada; execução integrada depende de configuração adicional.

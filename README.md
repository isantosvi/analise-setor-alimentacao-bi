# Projeto BI — Análise do Setor de Alimentação no Brasil

## Descrição

Este projeto tem como objetivo analisar dados de empresas do setor de alimentação no Brasil, utilizando Python para tratamento de dados e Power BI para construção de dashboards interativos. A análise busca identificar padrões de mercado, segmentação por atividade econômica, evolução ao longo do tempo e fatores relacionados ao encerramento de empresas.

---

## Objetivo

Responder às seguintes perguntas de negócio:

* Quantas empresas ativas existem no setor de alimentação?
* Quais segmentos (CNAEs) são mais e menos representativos?
* Houve crescimento ou declínio no número de empresas abertas ao longo dos anos?
* Quais são os principais motivos de empresas estarem baixadas ou inativas?

---

## Bases de Dados Utilizadas

Foram utilizadas três bases principais:

* **Estabelecimento**: contém informações cadastrais das empresas
* **CNAE**: descrição das atividades econômicas
* **Municípios**: dados de localização

---

## Tecnologias Utilizadas

* Python (pandas) para tratamento de dados
* Excel para ajustes complementares
* Power BI para modelagem e visualização

---

## Etapas do Projeto

### 1. Tratamento de Dados (Python e Excel)

* Leitura das bases com tratamento de encoding e separadores
* Padronização dos nomes das colunas
* Remoção de colunas desnecessárias
* Conversão de tipos (datas, números, texto)
* Tratamento de valores nulos e inconsistentes
* Preparação dos dados para análise

---

### 2. Modelagem no Power BI

* Importação da base tratada
* Criação de relacionamentos entre tabelas
* Criação de colunas calculadas e medidas DAX
* Organização das páginas do dashboard

---

## Estrutura do Dashboard

### Página 1 — Panorama do Setor

Apresenta uma visão geral do mercado:

* Total de empresas
* Quantidade de empresas ativas, baixadas e inapta
* Percentual de empresas ativas
* Distribuição por CNAE
* Distribuição das empresas por situação cadastral

Objetivo: entender o tamanho do mercado e sua composição.

---

### Página 2 — Evolução do Mercado

Apresenta a evolução das aberturas de empresas ao longo do tempo:

* Gráfico de linha com quantidade de aberturas por ano

Objetivo: identificar tendências de crescimento ou declínio no setor.

---

### Página 3 — Análise de Risco e Encerramento

Focada em entender o comportamento das empresas encerradas:

* Tempo de funcionamento até a baixa
* Distribuição geográfica das empresas encerradas
* Principais motivos de baixa/inatividade
* Evolução mensal de empresas suspensas e baixadas

Objetivo: identificar padrões de risco e causas de encerramento.

---

## Principais Métricas (DAX)

### Empresas Ativas

```DAX
EmpresasAtivas = 
CALCULATE(
    COUNTROWS(EmpresasAlimentacao),
    EmpresasAlimentacao[SituacaoCadastral] = "ATIVA"
)
```

### Quantidade de Aberturas

```DAX
QtdAberturas = COUNTROWS(EmpresasAlimentacao)
```

### Ano de Abertura

```DAX
AnoAbertura = YEAR(EmpresasAlimentacao[DataInicioAtividade])
```

---

## Principais Insights

* O setor de alimentação apresenta concentração em poucos segmentos, com destaque para lanchonetes e alimentação domiciliar
* Existe variação significativa na abertura de empresas ao longo dos anos
* A maior parte dos encerramentos ocorre entre 2 a 5 anos de funcionamento
* Os principais motivos de baixa estão relacionados a decisão voluntária, problemas fiscais e ausência de informações

---

## Limitações

* Possíveis inconsistências nos dados de origem
* Registros incompletos ou com valores nulos
* Dependência da qualidade dos dados cadastrais

---

## Próximos Passos

* Análise por região e comparação entre estados
* Cruzamento entre CNAE e taxa de encerramento
* Criação de indicadores preditivos de risco
* Evolução do dashboard para análises mais avançadas

---

## Conclusão

O projeto permitiu compreender melhor o comportamento do setor de alimentação no Brasil, identificando padrões relevantes de crescimento, segmentação e encerramento de empresas. A análise contribui para apoiar decisões estratégicas e identificar riscos no mercado.

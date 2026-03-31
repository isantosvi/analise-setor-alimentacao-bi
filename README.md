# Projeto BI — Análise do Setor de Alimentação no Brasil

## Sobre o Projeto

Este projeto foi desenvolvido com o objetivo de simular um cenário real de análise de dados no contexto de Business Intelligence.

A proposta surgiu da necessidade de consolidar conhecimentos em tratamento, modelagem e visualização de dados, aplicando essas etapas em um problema concreto. O setor de alimentação foi escolhido por apresentar alta competitividade e uma dinâmica relevante de abertura e encerramento de empresas, o que o torna ideal para análises exploratórias e geração de insights.

Mais do que construir um dashboard, o foco foi compreender o comportamento do mercado e identificar padrões que possam apoiar a tomada de decisão.

---

## Problema de Negócio

A análise busca responder questões relevantes para o entendimento do setor:

- Qual o volume de empresas ativas no segmento analisado  
- Quais atividades possuem maior representatividade  
- Como o mercado evoluiu ao longo do tempo  
- Quais fatores estão associados ao encerramento de empresas  

---

## Escopo da Análise

O projeto foi direcionado para CNAEs específicos do setor de alimentação:

- 4721102  
- 5611201  
- 5611203  
- 5611204  
- 5611205  
- 5620104  

Essa delimitação permite uma análise mais direcionada e coerente com o comportamento real do segmento.

---

## Bases de Dados Utilizadas

Foram utilizadas três bases principais:

- Estabelecimentos: informações cadastrais das empresas  
- CNAE: descrição das atividades econômicas  
- Municípios: dados de localização  

---

## Tecnologias Utilizadas

O projeto foi desenvolvido com ferramentas amplamente utilizadas no mercado de dados:

- Python (pandas) para tratamento, limpeza e integração dos dados  
- Excel para ajustes complementares e validações  
- Power BI para modelagem dos dados e construção dos dashboards  

---

## Processo de Desenvolvimento

### Tratamento de Dados

Nesta etapa foram realizados:

- Leitura e padronização dos arquivos  
- Correção de problemas de encoding e separadores  
- Limpeza de dados inconsistentes  
- Tratamento de valores nulos  
- Conversão de tipos de dados  
- Integração das bases (merge)  
- Preparação da base final para análise  

---

### Modelagem e Visualização

No Power BI, foram desenvolvidas:

- Estrutura de relacionamento entre tabelas  
- Indicadores de negócio  
- Organização do dashboard em páginas analíticas  
- Visualizações orientadas à tomada de decisão  

---

## Estrutura do Dashboard

### Página 1 — Panorama do Setor

Apresenta uma visão geral do mercado:

- Total de empresas  
- Distribuição por situação cadastral  
- Representatividade por atividade econômica  

Objetivo: compreender o tamanho e a composição do setor.

---

### Página 2 — Evolução do Mercado

Apresenta a evolução das aberturas de empresas ao longo do tempo.

Objetivo: identificar tendências de crescimento ou retração.

---

### Página 3 — Análise de Risco e Encerramento

Focada no comportamento das empresas encerradas:

- Tempo de funcionamento  
- Motivos de baixa/inatividade  
- Distribuição geográfica  
- Evolução de encerramentos  

Objetivo: identificar padrões de risco no setor.

---

## Principais Insights

- O setor apresenta concentração em determinados tipos de atividade  
- Existe variação relevante na abertura de empresas ao longo dos anos  
- Parte significativa das empresas encerra suas atividades nos primeiros anos  
- Os principais motivos de baixa estão associados a fatores operacionais e fiscais  

---

## Desafios Enfrentados

Durante o desenvolvimento do projeto, foram enfrentados desafios comuns em cenários reais de dados:

- Inconsistência nos dados de origem  
- Problemas de encoding nos arquivos  
- Necessidade de padronização de colunas  
- Tratamento de dados incompletos  

Esses pontos contribuíram diretamente para o desenvolvimento de habilidades práticas em análise de dados.

---

## Próximos Passos

- Análise comparativa entre regiões e estados  
- Cruzamento entre CNAE e taxa de encerramento  
- Evolução para modelos preditivos de risco  
- Estruturação de um pipeline de dados mais robusto  

---

## Conclusão

Este projeto representa uma aplicação prática do processo completo de análise de dados, desde o tratamento até a geração de insights.

A experiência permitiu consolidar conhecimentos técnicos e desenvolver uma visão mais analítica sobre dados de negócio, reforçando o interesse em atuar com Business Intelligence e análise de dados aplicada à tomada de decisão.

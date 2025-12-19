[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-blue.svg)](https://creativecommons.org/licenses/by/4.0/)

# Aplicação de Machine Learning na Formação Docente para Sistemas Adaptativos com Apoio de IA Generativa
## Um Estudo com Professores do Colégio Militar do Rio de Janeiro

Este repositório reúne os artefatos de pesquisa, dados tratados e scripts de análise do estudo que investiga a aplicação de técnicas de **Machine Learning** no contexto da **formação docente**, com foco na preparação de professores para atuação com **sistemas adaptativos** e com apoio de **Inteligência Artificial Generativa**.

O estudo foi conduzido a partir de um **workshop formativo** realizado com professores do **Colégio Militar do Rio de Janeiro (CMRJ)**, e tem como objetivo analisar perfis docentes, padrões de aprendizagem e percepções sobre o uso de IA na educação.

---

## Visão Geral do Estudo

- **Participantes:** 47 professores
- **Contexto:** Workshop de formação docente 2025
- **Instituição:** Colégio Militar do Rio de Janeiro (CMRJ)
- **Abordagem:** Análise quantitativa com técnicas de aprendizado não supervisionado

---

## Metodologia Analítica

As seguintes técnicas e procedimentos foram utilizados:

- Normalização dos dados por **Z-score**
- **Clusterização K-means** com definição de `k = 3`
- Identificação de três perfis docentes (A, B e C)
- **Análise de Componentes Principais (PCA)** para visualização dos clusters
- **ANOVA unidirecional** para comparação entre grupos
- Teste **post hoc de Tukey HSD**
- Análise de correlação entre variáveis
- Questionário de percepção em escala **Likert**
- Avaliação de confiabilidade do instrumento por **Alpha de Cronbach (α = 0.8756)**

---

## Perfis Identificados

A aplicação do algoritmo K-means resultou nos seguintes perfis:

- **Perfil A:** 19 professores
- **Perfil B:** 11 professores
- **Perfil C:** 17 professores

A caracterização pedagógica e estatística desses perfis é apresentada e discutida no artigo científico associado a este repositório.

---

## Estrutura do Repositório

```text

├── datasets/
│   ├── autoavaliacao_e_percepcao.xlsx
│   ├── diagnostico.xlsx
│   └── info.txt
├── LICENSE
├── README.md
├── machine_learning_formacao_docente.ipynb
└── requirements.txt
```

## ▶️ Reproduzindo as Análises

### Requisitos

- Python 3.10 ou superior
- Ambiente Jupyter (local ou Google Colab)

### Bibliotecas Utilizadas

- `numpy`
- `pandas`
- `scipy`
- `scikit-learn`
- `matplotlib`
- `statsmodels`

### Instalação das Dependências

```bash
pip install -r requirements.txt
```

### Execução

1. Abra o notebook principal:
   - `notebooks/analise_ml_formacao_docente.ipynb`

2. Execute todas as células **na ordem**, para:
   - carregar os dados
   - aplicar o pré-processamento
   - realizar a clusterização com **K-means (k = 3)**
   - gerar visualizações por **PCA**
   - aplicar **ANOVA unidirecional** e **Tukey HSD**
   - calcular o **Alpha de Cronbach**
   - exportar tabelas e figuras

3. Os arquivos gerados serão salvos nos diretórios:
   - `results/tabelas/`
   - `results/figuras/`

## Principais Resultados

- Diferenças estatisticamente significativas entre os clusters  
  (**ANOVA:** F = 9.059, *p* < 0.001)

- O teste **Tukey HSD** indicou que os **Perfis A e B** apresentaram ganhos significativamente maiores que o **Perfil C**

- O instrumento de percepção apresentou **alta confiabilidade interna**  
  (**α de Cronbach = 0.8756**)

---

## Ciência Aberta e Reprodutibilidade

Este repositório foi organizado com foco em **transparência**, **reprodutibilidade** e **ciência aberta**, disponibilizando:

- dados organizados (brutos e tratados)
- scripts de análise
- notebooks executáveis
- figuras e tabelas exportáveis

Dados sensíveis foram devidamente **anonimizados**, em conformidade com princípios éticos de pesquisa com seres humanos.

---

## Declaração de Uso de Inteligência Artificial

Ferramentas de **IA generativa** foram utilizadas como apoio à organização do código, documentação e revisão textual, sem substituir a autoria intelectual, a análise estatística ou a interpretação científica dos resultados.

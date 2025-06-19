# 📦 Projeto de Previsão de Demanda com Data Lake em Camadas

Este projeto demonstra a construção de um pipeline de dados baseado em um **Data Lake estruturado por camadas**, com foco na **previsão de demanda de produtos**. Foi desenvolvido com boas práticas de engenharia e ciência de dados, simulando um ambiente produtivo.

---

## 🎯 Objetivo

Criar uma arquitetura robusta de ingestão, transformação e disponibilização de dados para suportar análises e modelagem preditiva, com foco em:

- Governança e rastreabilidade dos dados
- Modularidade e reuso em diferentes estágios do pipeline
- Preparação eficiente de dados para modelos de machine learning

---

## 🏗️ Arquitetura do Data Lake

O Data Lake é organizado em **camadas** com responsabilidades bem definidas:

| Camada     | Descrição |
|------------|-----------|
| **Ingestion** | Armazena os **dados brutos originais**, exatamente como foram recebidos. |
| **Raw** | Dados com **pequenas padronizações**, como renomeação de colunas e conversão de tipos. |
| **Trusted** | Camada onde ocorre a **engenharia de variáveis** com regras de negócio e agregações temporais. |
| **Refined** | Dados **prontos para consumo analítico ou alimentar modelos** de machine learning. |
| **Metadados** | Documentação automatizada com estatísticas descritivas de cada variável (nulos, tipos, cardinalidade, etc). |

---

## ⚙️ Funcionalidades Implementadas

- 📥 Ingestão simulada a partir de arquivos `.csv` e `.parquet`
- 🧼 Padronização de dados e tratamento de tipos
- 🧠 Feature engineering com janelas de tempo, agregações e frequências
- 📊 Análises exploratórias para apoiar a modelagem
- 🧾 Geração de metadados automatizados por DataFrame
- 💾 Escrita de dados em formato Parquet por camadas organizadas
- 🧪 Construção de janelas de observação e previsão para modelagem futura

---

## 🧰 Tecnologias e Bibliotecas Utilizadas

- **Apache Spark (PySpark)** – Processamento de dados em larga escala
- **Python 3.10+** – Linguagem base do projeto
- **Java JDK 11** – Requisito para o funcionamento do Spark
- **Google Colab** – Ambiente de desenvolvimento e execução
- **Google Drive** – Simulação de armazenamento em nuvem
- **findspark** – Integração entre Spark e Colab
- **pandas / matplotlib / seaborn** – Análise e visualização de dados

---

## 🗂️ Estrutura de Diretórios

````bash
DADOS/
├── INGESTION/       # Dados brutos originais
├── RAW/             # Dados padronizados
├── TRUSTED/         # Feature engineering e regras de negócio
├── REFINED/         # Dados prontos para consumo analítico/modelagem
└── METADADOS/       # Estatísticas e dicionários de variáveis
````

# 🧪 Execução no Google Colab

Para configurar o ambiente,basta executar essa linha:
!pip install -q findspark pyspark

Caso o processamento seja feito em outro local, precisa instalar as versões utilizadas, abaixo:

# Instalar Java e Spark
!apt-get install openjdk-11-jdk-headless -qq

!wget -q https://downloads.apache.org/spark/spark-3.3.2/spark-3.3.2-bin-hadoop3.tgz

!tar xf spark-3.3.2-bin-hadoop3.tgz




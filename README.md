# pipeline-olist-databricks

# 🛒 Pipeline de Engenharia de Dados - Olist E-commerce

Projeto "End-to-End" de Engenharia de Dados construído para processar dados públicos do E-commerce Brasileiro (Olist). O objetivo foi construir um Data Lakehouse utilizando a arquitetura Medallion (Bronze, Silver, Gold).

## 🛠 Tecnologias Utilizadas
- **Language:** Python (PySpark)
- **Engine:** Azure Databricks (Spark Cluster)
- **Storage:** Databricks File System (DBFS) / Unity Catalog
- **Format:** Delta Lake (Parquet versionado)
- **Orchestration:** Databricks Notebooks

## 🏗 Arquitetura do Projeto
O pipeline segue a arquitetura **Medallion**:
1.  **Bronze:** Ingestão "Raw" dos dados CSV originais para Delta Lake.
2.  **Silver:** Limpeza, tipagem de dados (Casting), renomeação de colunas e tratamento de nulos.
3.  **Gold:** Agregações de negócio (Joins e KPIs) para responder perguntas como "Faturamento Diário" e "Top Categorias".

## 📊 Resultados
> (Aqui você pode colocar aquele print do gráfico de vendas que geramos!)
*O gráfico acima demonstra o pico de vendas identificado na Black Friday de 2017.*

## 🚀 Como Executar
1. Clone este repositório.
2. Faça upload dos arquivos da pasta `data` para o seu Databricks Volume.
3. Execute os notebooks na ordem numérica (01 -> 02 -> 03).

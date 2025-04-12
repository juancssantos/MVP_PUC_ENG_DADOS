# Data Warehouse para Análise de Transações com Cartões de Pagamento do Governo Federal (CPGF)

Link: https://databricks-prod-cloudfront.cloud.databricks.com/public/4027ec902e239c93eaaa8714f173bcfc/2894892977690218/2204695551162580/1473597321450676/latest.html

<img width="784" alt="print databricks" src="https://github.com/user-attachments/assets/29f16581-7829-4eb8-8cdb-397686df5666" />

📌 Visão Geral

Este projeto implementa um Data Warehouse no Databricks para análise de transações realizadas com cartões de pagamento do governo federal (CPGF), utilizando dados abertos do Portal da Transparência.

O modelo segue um esquema estrela (star schema), otimizado para consultas analíticas rápidas, com:

1 tabela fato (fato_transacoes) contendo métricas como valor, data e chaves de relacionamento.

4 tabelas de dimensão (dim_tipo_cartao, dim_estabelecimento, dim_unidade_gestora, dim_portador) para contextualização dos dados.

🎯 Objetivos

✅ ETL Automatizado

Extração de dados de arquivos CSV (*_CPGF.csv).

Tratamento de paginação e validação de integridade.

✅ Modelagem Dimensional (Star Schema)

Chaves primárias únicas e sem duplicatas.

Validação de campos obrigatórios (não nulos).

Consistência de valores monetários e datas.

✅ Otimização para Performance

Particionamento por data.

Z-Ordering para consultas mais rápidas.

Atualização de estatísticas para melhor execução no Spark.

✅ Documentação e Rastreabilidade

Catálogo de dados detalhando tabelas e campos.

Linhagem dos dados (origem → transformação → destino).

⚙️ Tecnologias Utilizadas

Databricks (Spark SQL)

Python (PySpark, Pandas para validações)


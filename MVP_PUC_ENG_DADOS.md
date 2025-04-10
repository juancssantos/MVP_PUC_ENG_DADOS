Documentação do Modelo de Dados
# Data Model Documentation

## Table: date_series

**Row count:** 3,651

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| date | DateType() | Date field |
| year | IntegerType() | No description available |
| month | IntegerType() | No description available |
| day | IntegerType() | No description available |
| day_of_week | IntegerType() | No description available |
| day_of_year | IntegerType() | No description available |
| week_of_year | IntegerType() | No description available |
| quarter | IntegerType() | No description available |
| is_weekend | BooleanType() | No description available |

## Table: dim_estabelecimento

**Row count:** 11,711

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| ID_ESTABELECIMENTO | LongType() | Identifier field |
| CNPJ_OU_CPF_FAVORECIDO | StringType() | Identifier field |
| NOME_FAVORECIDO | StringType() | Identifier field |
| DATA_INICIO_VIGENCIA | DateType() | No description available |
| DATA_FIM_VIGENCIA | DateType() | No description available |
| CURRENT_FLAG | BooleanType() | No description available |

## Table: dim_portador

**Row count:** 3,025

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| ID_PORTADOR | LongType() | Identifier field |
| CPF_PORTADOR | StringType() | No description available |
| NOME_PORTADOR | StringType() | No description available |
| DATA_INICIO_VIGENCIA | DateType() | No description available |
| DATA_FIM_VIGENCIA | DateType() | No description available |
| CURRENT_FLAG | BooleanType() | No description available |

## Table: dim_tempo

**Row count:** 125

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| ID_TEMPO | IntegerType() | Identifier field |
| DATA | DateType() | No description available |
| DIA | IntegerType() | No description available |
| MES | IntegerType() | No description available |
| ANO | IntegerType() | No description available |
| TRIMESTRE | IntegerType() | No description available |
| SEMESTRE | IntegerType() | No description available |
| DIA_SEMANA | IntegerType() | No description available |
| NOME_DIA_SEMANA | StringType() | No description available |
| NOME_MES | StringType() | No description available |
| FERIADO | BooleanType() | No description available |
| FIM_DE_SEMANA | BooleanType() | No description available |

## Table: dim_tipo_cartao

**Row count:** 3

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| ID_TIPO_CARTAO | IntegerType() | Identifier field |
| TIPO_TRANSACAO | StringType() | No description available |
| DESCRICAO_TRANSACAO | StringType() | No description available |
| DATA_INICIO_VIGENCIA | DateType() | No description available |
| DATA_FIM_VIGENCIA | DateType() | No description available |
| CURRENT_FLAG | BooleanType() | No description available |

## Table: dim_unidade_gestora

**Row count:** 879

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| ID_UNIDADE_GESTORA | LongType() | Identifier field |
| CODIGO_UNIDADE_GESTORA | StringType() | Identifier field |
| NOME_UNIDADE_GESTORA | StringType() | Identifier field |
| CODIGO_ORGAO | StringType() | No description available |
| NOME_ORGAO | StringType() | No description available |
| CODIGO_ORGAO_SUPERIOR | StringType() | No description available |
| NOME_ORGAO_SUPERIOR | StringType() | No description available |
| DATA_INICIO_VIGENCIA | DateType() | No description available |
| DATA_FIM_VIGENCIA | DateType() | No description available |
| CURRENT_FLAG | BooleanType() | No description available |

## Table: fato_transacoes

**Row count:** 34,999

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| ID_TRANSACAO | LongType() | Identifier field |
| ID_TIPO_CARTAO | IntegerType() | Identifier field |
| ID_ESTABELECIMENTO | LongType() | Identifier field |
| ID_UNIDADE_GESTORA | LongType() | Identifier field |
| ID_PORTADOR | LongType() | Identifier field |
| ID_TEMPO | IntegerType() | Identifier field |
| ANO_EXTRATO | IntegerType() | No description available |
| MES_EXTRATO | IntegerType() | No description available |
| VALOR_TRANSACAO | DecimalType(18,2) | No description available |
| DATA_TRANSACAO | DateType() | No description available |
| DATA_CARGA | TimestampType() | No description available |

## Table: date_series

**Row count:** 3,651

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| date | DateType() | Date field |
| year | IntegerType() | No description available |
| month | IntegerType() | No description available |
| day | IntegerType() | No description available |
| day_of_week | IntegerType() | No description available |
| day_of_year | IntegerType() | No description available |
| week_of_year | IntegerType() | No description available |
| quarter | IntegerType() | No description available |
| is_weekend | BooleanType() | No description available |
# Customer Personality Analysis
Analysis of company's ideal customers

## **Sobre o conjunto de dados**

### **Contexto**

**Declaração do problema**

A análise de personalidade do cliente é uma análise detalhada dos clientes ideais de uma empresa. Ela ajuda uma empresa a entender melhor seus clientes e facilita a modificação de produtos de acordo com as necessidades, comportamentos e preocupações específicas de diferentes tipos de clientes.

A análise de personalidade do cliente ajuda uma empresa a modificar seu produto com base em seus clientes-alvo de diferentes tipos de segmentos de clientes. Por exemplo, em vez de gastar dinheiro para comercializar um novo produto para cada cliente no banco de dados da empresa, uma empresa pode analisar qual segmento de clientes tem mais probabilidade de comprar o produto e, então, comercializá-lo apenas naquele segmento específico.

### **Conteúdo**

### **Tabela: Pessoas**
| **Coluna**        | **Descrição**                                                                         |
|-------------------|---------------------------------------------------------------------------------------|
| **ID**            | Identificador exclusivo do cliente.                                                  |
| **Ano_Nascimento**| Ano de nascimento do cliente.                                                        |
| **Educação**      | Nível de educação do cliente.                                                        |
| **Estado civil**  | Estado civil do cliente.                                                             |
| **Renda**         | Renda familiar anual do cliente.                                                     |
| **Kidhome**       | Número de crianças na casa do cliente.                                               |
| **Teenhome**      | Número de adolescentes na casa do cliente.                                           |
| **Dt_Cliente**    | Data de inscrição do cliente na empresa.                                             |
| **Ano**           | Ano da última compra do cliente.                                                     |
| **Mês**           | Mês da última compra do cliente.                                                     |
| **Dia**           | Dia da última compra do cliente.                                                     |
| **Idade**         | Idade do cliente, calculada a partir do ano de nascimento e da data de inscrição.     |
| **Recência**      | Número de dias desde a última compra do cliente.                                     |
| **Reclamação**    | Indica se o cliente reclamou nos últimos 2 anos (1 para sim, 0 para não).            |
| **Filhos**        | Número de filhos do cliente.                                                         |
| **TamanhoFamília**| Tamanho total da família do cliente, incluindo ele mesmo e seus dependentes.          |
| **EstáCasado**    | Indica se o cliente está casado (1 para sim, 0 para não).                            |
| **Senioridade**   | Número de dias desde que o cliente se inscreveu na empresa.                          |

### **Tabela: Produtos**
| **Coluna**          | **Descrição**                                                          |
|---------------------|----------------------------------------------------------------------|
| **MntWines**         | Valor gasto em vinho nos últimos 2 anos.                             |
| **MntFruits**        | Valor gasto em frutas nos últimos 2 anos.                            |
| **MntMeatProducts**  | Valor gasto em carne nos últimos 2 anos.                             |
| **MntFishProducts**  | Valor gasto em peixe nos últimos 2 anos.                             |
| **MntSweetProducts** | Valor gasto em doces nos últimos 2 anos.                             |
| **MntGoldProds**     | Valor gasto em ouro nos últimos 2 anos.                              |
| **TotalMntSpent**    | Total gasto em todos os produtos nos últimos 2 anos.                 |
| **TotalCompras**     | Total de compras feitas nos últimos 2 anos.                          |
| **ValorMédiaCompra** | Valor médio das compras feitas nos últimos 2 anos.                   |

### **Tabela: Promoção**
| **Coluna**            | **Descrição**                                                                  |
|-----------------------|-------------------------------------------------------------------------------|
| **NumDealsPurchases** | Número de compras feitas com desconto.                                       |
| **AcceptedCmp1**      | Indica se o cliente aceitou a oferta na 1ª campanha (1 para sim, 0 para não). |
| **AcceptedCmp2**      | Indica se o cliente aceitou a oferta na 2ª campanha (1 para sim, 0 para não). |
| **AcceptedCmp3**      | Indica se o cliente aceitou a oferta na 3ª campanha (1 para sim, 0 para não). |
| **AcceptedCmp4**      | Indica se o cliente aceitou a oferta na 4ª campanha (1 para sim, 0 para não). |
| **AcceptedCmp5**      | Indica se o cliente aceitou a oferta na 5ª campanha (1 para sim, 0 para não). |
| **Resposta**          | Indica se o cliente aceitou a oferta na última campanha (1 para sim, 0 para não).|

### **Tabela: Local**
| **Coluna**             | **Descrição**                                                   |
|------------------------|---------------------------------------------------------------|
| **NumWebPurchases**     | Número de compras feitas pelo site da empresa.               |
| **NumCatalogPurchases** | Número de compras feitas usando um catálogo.                 |
| **NumStorePurchases**   | Número de compras feitas diretamente em lojas.               |
| **NumWebVisitsMonth**   | Número de visitas ao site da empresa no último mês.          |
| **WebVsStorePurchases** | Relação entre compras feitas no site e em lojas físicas.     |


### **Alvo**

Precisa realizar clustering para resumir segmentos de clientes.

## Primeiras linhas do Dataset:

| ID   | Year_Birth | Education | Marital_Status | Income | Kidhome | Teenhome | Dt_Customer | Recency | MntWines | MntFruits | MntMeatProducts | MntFishProducts | MntSweetProducts | MntGoldProds | NumDealsPurchases | NumWebPurchases | NumCatalogPurchases | NumStorePurchases | NumWebVisitsMonth | AcceptedCmp3 | AcceptedCmp4 | AcceptedCmp5 | AcceptedCmp1 | AcceptedCmp2 | Complain | Z_CostContact | Z_Revenue | Response |
|------|------------|-----------|----------------|--------|---------|----------|-------------|---------|----------|-----------|-----------------|-----------------|------------------|--------------|-------------------|-----------------|---------------------|-------------------|------------------|--------------|--------------|--------------|--------------|--------------|----------|---------------|-----------|----------|
| 5524 | 1957       | Graduation| Single         | 58138  | 0       | 0        | 04-09-2012  | 58      | 635      | 88        | 546             | 172             | 88               | 88           | 3                 | 8               | 10                  | 4                 | 7                | 0            | 0            | 0            | 0            | 0            | 3        | 11            | 1         |
| 2174 | 1954       | Graduation| Single         | 46344  | 1       | 1        | 08-03-2014  | 38      | 11       | 1         | 6               | 2               | 1                | 6            | 2                 | 1               | 1                   | 2                 | 5                | 0            | 0            | 0            | 0            | 0            | 3        | 11            | 0         |
| 4141 | 1965       | Graduation| Together       | 71613  | 0       | 0        | 21-08-2013  | 26      | 426      | 49        | 127             | 111             | 21               | 42           | 1                 | 8               | 2                   | 10                | 4                | 0            | 0            | 0            | 0            | 0            | 3        | 11            | 0         |
| 6182 | 1984       | Graduation| Together       | 26646  | 1       | 0        | 10-02-2014  | 26      | 11       | 4         | 20              | 10              | 3                | 5            | 2                 | 2               | 0                   | 4                 | 6                | 0            | 0            | 0            | 0            | 0            | 3        | 11            | 0         |
| 5324 | 1981       | PhD       | Married        | 58293  | 1       | 0        | 19-01-2014  | 94      | 173      | 43        | 118             | 46              | 27               | 15           | 5                 | 5               | 3                   | 6                 | 5                | 0            | 0            | 0            | 0            | 0            | 3        | 11            | 0         |

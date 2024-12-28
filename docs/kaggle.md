# **Sobre o conjunto de dados**

### **Contexto**

**Declaração do problema**

A análise de personalidade do cliente é uma análise detalhada dos clientes ideais de uma empresa. Ela ajuda uma empresa a entender melhor seus clientes e facilita a modificação de produtos de acordo com as necessidades, comportamentos e preocupações específicas de diferentes tipos de clientes.

A análise de personalidade do cliente ajuda uma empresa a modificar seu produto com base em seus clientes-alvo de diferentes tipos de segmentos de clientes. Por exemplo, em vez de gastar dinheiro para comercializar um novo produto para cada cliente no banco de dados da empresa, uma empresa pode analisar qual segmento de clientes tem mais probabilidade de comprar o produto e, então, comercializá-lo apenas naquele segmento específico.

### **Conteúdo**

**Atributos**

**Pessoas**

- **ID**: identificador exclusivo do cliente
- **Ano_Nascimento**: ano de nascimento do cliente
- **Educação**: nível de educação do cliente
- **Estado civil**: estado civil do cliente
- **Renda**: renda familiar anual do cliente
- **Kidhome**: número de crianças na casa do cliente
- **Teenhome**: número de adolescentes na casa do cliente
- **Dt_Cliente**: data de inscrição do cliente na empresa
- **Recência**: número de dias desde a última compra do cliente
- **Reclamação**: 1 se o cliente reclamou nos últimos 2 anos, 0 caso contrário

**Produtos**

- **MntWines**: valor gasto em vinho nos últimos 2 anos
- **MntFruits**: valor gasto em frutas nos últimos 2 anos
- **MntMeatProducts**: valor gasto em carne nos últimos 2 anos
- **MntFishProducts**: valor gasto em peixe nos últimos 2 anos
- **MntSweetProducts**: valor gasto em doces nos últimos 2 anos
- **MntGoldProds**: valor gasto em ouro nos últimos 2 anos

**Promoção**

- **NumDealsPurchases**: número de compras feitas com desconto
- **AcceptedCmp1**: 1 se o cliente aceitou a oferta na 1ª campanha, 0 caso contrário
- **AcceptedCmp2**: 1 se o cliente aceitou a oferta na 2ª campanha, 0 caso contrário
- **AcceptedCmp3**: 1 se o cliente aceitou a oferta na 3ª campanha, 0 caso contrário
- **AcceptedCmp4**: 1 se o cliente aceitou a oferta na 4ª campanha, 0 caso contrário
- **AcceptedCmp5**: 1 se o cliente aceitou a oferta na 5ª campanha, 0 caso contrário
- **Resposta**: 1 se o cliente aceitou a oferta na última campanha, 0 caso contrário

**Local**

- **NumWebPurchases**: número de compras feitas pelo site da empresa
- **NumCatalogPurchases**: número de compras feitas usando um catálogo
- **NumStorePurchases**: número de compras feitas diretamente em lojas
- **NumWebVisitsMonth**: número de visitas ao site da empresa no último mês

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


# **Customer Personality Analysis**

[Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)

[Customer Segmentation Clustering by Kevin](https://www.kaggle.com/code/kebinnuil/customer-segmentation-clustering-by-kevin)

[🛍 Customer Analysis| EDA | Profiling | KMeans](https://www.kaggle.com/code/visitnehaverma/customer-analysis-eda-profiling-kmeans)

[💼 Customer Personality Analysis: 🎯 Unsupervised](https://www.kaggle.com/code/sajjadalishah/customer-personality-analysis-unsupervised)

[Customer EDA | Clustering | Strategies](https://www.kaggle.com/code/marcelobatalhah/customer-eda-clustering-strategies)

[Clustering | Customer personality analysis](https://www.kaggle.com/code/a7madmostafa/clustering-customer-personality-analysis)

[market segmentation analysis](https://www.kaggle.com/code/taylorwill/market-segmentation-analysis)

[Customer Personality Analysis with Python | Thecleverprogrammer](https://thecleverprogrammer.com/2021/02/08/customer-personality-analysis-with-python/)

- Datasets
    
    [Customer Segmentation: Clustering 🛍️🛒🛒](https://www.kaggle.com/code/karnikakapoor/customer-segmentation-clustering)
    
    [Wine Dataset for Clustering](https://www.kaggle.com/datasets/harrywang/wine-dataset-for-clustering)
    
    [Credit Card Customer Data](https://www.kaggle.com/datasets/aryashah2k/credit-card-customer-data)
    
    [Household Electric Power Consumption](https://www.kaggle.com/datasets/uciml/electric-power-consumption-data-set)
    
    [Mall Customers Segmentation](https://www.kaggle.com/datasets/abdallahwagih/mall-customers-segmentation)
    
    [Bank Customer Segmentation (1M+ Transactions)](https://www.kaggle.com/datasets/shivamb/bank-customer-segmentation)
    
    [Social Media Usage and Emotional Well-Being](https://www.kaggle.com/datasets/emirhanai/social-media-usage-and-emotional-well-being)
    
    [Customer Clustering](https://www.kaggle.com/datasets/dev0914sharma/customer-clustering)
    
    [Fish species sampling data - legnth and weight](https://www.kaggle.com/datasets/taweilo/fish-species-sampling-weight-and-height-data)
    
    [Search | Kaggle](https://www.kaggle.com/search?q=clustering+dataset+in%3Adatasets)
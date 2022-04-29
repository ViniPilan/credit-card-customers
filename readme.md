# Problemas com clientes de uma empresa de cartão de crédito

## Criando meios para evitá-los e um modelo preditivo para identificá-los antes mesmo de acontecerem


### Introdução
Empresas de cartão de crédito exercem a função de intermediador financeiro entre duas partes, sendo uma delas alguma determinada empresa e a outra o consumidor. A empresa de cartão de crédito envia o dinheiro para essa determinada empresa antes mesmo de receber o montante do cliente, o qual fica com essa dívida em seu cartão. 

![img_inicial](Imagens/img_inicio.jpg)


Por essa razão, clientes que geram problemas para a empresa de crédito podem acarretar em prejuízos para a mesma, já que ela fica a espera de receber o dinheiro de seu cliente para pagar sua dívida.

Em virtude disso, é de grande importância para a empresa ter conhecimento de **meios preventivos para diminuir a chance de algum de seus clientes cause problemas**, já que problema pode ser visto como sinônimo de prejuízo nesses casos. Neste documento foram criados:
- *insights* para reduzir os clientes que geram problemas para a empresa

- um modelo capaz de estimar a probabilidade de determinado cliente vir a causar problemas para a empresa.


### Resultados e Soluções
A análise exploratória feita sobre os dados resultou em alguns *insights* e na criação de um modelo classificador de machine learning que estima a probabilidade de um cliente gerar problemas para a empresa e, de acordo com isso, o classifica como problemático ou não. Os insights e hipóteses, assim como mais informações sobre o modelo criado podem ser encontradas no arquivo 'Análise Explanatória - Resultados' (ou clicando [aqui](AnáliseExplanatória-Resultados.pdf)).


### Estrutura do projeto
o projeto consiste na análise exploratória dos dados, na síntese de um modelo preditivo que estima a probabilidade de determinado cliente causar ou não problemas e a apresentação de todos os resultados, incluíndo *insights* que podem funcionar como medidas preventivas para reduzir o número de clientes que geram problemas. 

A pasta **Dados** contém todos os dados utilizados na análise. O data set original está contido no arquivo *BankChurners.csv* e mais informações sobre o mesmo podem ser encontradas mais abaixo deste documento. O arquivo *BankChurners_preprocessed.csv* contém os dados do data set original porém pré processados. Mais informações sobre ele podem sem encontradas no notebook da análise exploratória.

A pasta **Notebooks** contém todos os jupyter notebooks desenvolvidos. O notebook *AnáliseExploratória&Modelagem* apresenta o pré e o processamento dos dados do data set, como também o processo de modelagem e avaliação. O modelo criado tem como base o algoritmo de Regressão Logística e apresentou bons resultados de classificação.

A pasta **Imagens** contém todas as imagens geradas na análise exploratória e na análise explanatória.

A pasta **Arquivos** contém o documento .docx utilizado para sintetizar o relatório da análise explanatória, e contém também mais dois arquivos binários .pickle que armazenam o modelo ajustado de machine learning e o escalador utilizado para normalizar os dados do data set processado.


### Informações técnicas sobre os dados utilizados

Os dados utilizados (mencionados como *data set original* no tópico acima) são do data set [Credit Card Customers](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers) do Kaggle. Informações sobre cada *feature* podem ser vistas abaixo:

Nome da coluna | Conteúdo
---------|---------
CLIENTNUM | Client number. Unique identifier for the customer holding the account 
Attrition_Flag | Internal event (customer activity) variable - if the account is closed then 1 else 0
Customer_Age | Demographic variable - Customer's Age in Years
Gender | Demographic variable - M=Male, F=Female
Dependent_count | Demographic variable - Number of dependents
Education_Level | Demographic variable - Educational Qualification of the account holder example: high school, college graduate, etc.)
Marital_Status | Demographic variable - Married, Single, Divorced, Unknown
Income_Category | Demographic variable - Annual Income Category of the account holder (< $40K, $40K - 60K, $60K - $80K, $80K-$120K, > $120K, Unknown)
Card_Category | Product Variable - Type of Card (Blue, Silver, Gold, Platinum)
Months_on_book | Period of relationship with bank
Total_Relationship_Count | Total no. of products held by the customer
Months_Inactive_12_mon | No. of months inactive in the last 12 months
Contacts_Count_12_mon | No. of Contacts in the last 12 months
Credit_Limit | Credit Limit on the Credit Card
Total_Revolving_Bal | Total Revolving Balance on the Credit Card
Avg_Open_To_Buy | Open to Buy Credit Line (Average of last 12 months)
Total_Amt_Chng_Q4_Q1 | Change in Transaction Amount (Q4 over Q1)
Total_Trans_Amt | Total Transaction Amount (Last 12 months)
Total_Trans_Ct | Total Transaction Count (Last 12 months)
Total_Ct_Chng_Q4_Q1 | Change in Transaction Count (Q4 over Q1)
Avg_Utilization_Ratio | Average Card Utilization Ratio


### Sobre o autor deste projeto
Me chamo Vinícius, sou fascinado pela ciência de dados e encontrei nessa área uma paixão. Busco aprender constantemente para alcançar autoridade como Cientista de Dados profissional e atingir este que é meu objetivo de carreira.

Estudo Ciência da Computação na UNESP Bauru (estou no último ano do curso, tenho horários bastante flexíveis) e venho estudando ciência de dados para conseguir me consolidar no mercado.

Já realizei cursos, adquiri certificações e desenvolvi alguns projetos que envolvem e misturam conceitos como Python, análise e visualização de dados, Machine Learning (classificação, regressão, otimização, agrupamento), Deep Learning e SQL.

Tenho um site pessoal que contém mais informações sobre mim, minhas principais certificações e projetos: https://sites.google.com/view/vinicius-pilan/
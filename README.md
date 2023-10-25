

# Previsão de Churn: Identificação e Estratégias de Retenção

## Previsão de Churn
Este projeto traz à luz uma análise abrangente sobre a retenção de clientes em um mercado de serviços telefônicos. A previsão de Churn é fundamental para as empresas porque permite a identificação antecipada de clientes em risco de saída, reduzindo perdas financeiras, melhorando a satisfação do cliente, direcionando eficazmente recursos de retenção, e impulsionando a rentabilidade, o que é essencial para a sustentabilidade e o sucesso a longo prazo. Nesse sentido, a construção de um modelo de Machine Learning, conjuntamente ao uso de técnicas estatísticas, permite solucionar problemas relativos à perda de clientes e, dessa forma, promove um aumento dos lucros da empresa, sustentando suas atividades num amplo contexto.

A base de dados utilizada está disponível aqui: [Telco Customer Churn](https://www.kaggle.com/blastchar/telco-customer-churn)

## Objetivo
O objetivo deste projeto é construir um modelo de Machine Learning que seja capaz de identificar os clientes que são propensos a saírem da empresa, servindo como base para a tomada de decisão da empresa de telefonia aqui apresentada. Por outro lado, a análise construída também almeja fornecer sustentação à formulação de estratégias de retenção de clientes por meio do mapeamento e segmentação dos clientes propensos ao churn.

## Requisitos
Neste projeto, foi utilizada a versão 3.11.4 do Python

A versão do pip utilizada é a 23.3.1

A versão do git utilizada é a 2.42.0

Demais requisitos se encontram no arquivo requirements.txt

## Replicação
> [!NOTE]
> Para utilizar este projeto, é necessário clonar o repositório
```
git clone https://github.com/lazarocordeirosilva/Previsao_Churn.git
```
> [!NOTE]
> Após isso, você pode instalar os pacotes nas versões utilizadas
```
pip install -r requirements.txt
```

## Processamento
O projeto contempla as seguintes etapas:
* Manipulação de Dados Inicial
* EDA
* Codificação de Variáveis (OHE e OE)
* Teste de Performance em Diferentes Abordagens de Imputação 
* Utilização de Cross-Validation para competição de modelos
* Uso de Feature Engineering Para Aumentar Performance
* Otimização de Hiperparâmetros
* Avaliação do Modelo

## Principais Conclusões e Resultados
Clientes mais propensos ao Churn:
* Não possuem dependentes
* Possuem acesso à internet por meio de fibra óptica
* Possuem múltiplas linhas telefônicas

No que diz respeito a modelagem preditiva, foi possível obter uma taxa de verdadeiros positivos de 78,82% 
Os erros do tipo falso negativo, como esperado, foram os menores. Eles representam aproximadamante 22% dos erros totais
Ao focar na métrica de avaliação que contemplasse o desbalanceamento de classes, durante o processo de Cross-Validation, foi possível atingir um f1-score de 62,19 no conjunto de teste

## Estrutura do Projeto

```
├── LICENSE
├── README.md               <- README.md com principais informações do projeto.
├── data
│   ├── data dictionary     <- Dicionário dos dados utilizados no projeto.
│   └── raw                 <- Base de dados bruta (original).
├── notebook                <- Jupyter notebook contendo toda a manipulação de dados e modelagem.
├── requisitos              <- Todas as bibiliotecas utilizadas (em cada versão). Arquivo gerado com 'pip freeze > requirements.txt'

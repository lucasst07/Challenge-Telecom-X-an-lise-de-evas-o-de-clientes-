## Challenge-Telecom-X-analise-de-evasao-de-clientes-
Um desafio do programa ONE da Oracle com parceria com a Alura

# Análise de Evasão de Clientes (Churn) - TelecomX

## 📖 Visão Geral do Projeto

Este repositório contém uma análise exploratória de dados (EDA) sobre a evasão de clientes (churn) em uma empresa fictícia do setor de telecomunicações, a TelecomX. O principal objetivo deste projeto é identificar os fatores e padrões de comportamento que mais influenciam a decisão de um cliente cancelar seus serviços.

A partir dos insights gerados, o projeto busca fornecer uma base sólida para a criação de estratégias de retenção mais eficazes, visando reduzir a taxa de churn e aumentar a lealdade dos clientes.

## 📊 Dataset

O conjunto de dados utilizado foi fornecido em formato JSON e contém informações sobre o perfil dos clientes, os serviços contratados e o status de evasão. Os dados foram extraídos da seguinte fonte:

- **URL:** `https://raw.githubusercontent.com/alura-cursos/challenge2-data-science/refs/heads/main/TelecomX_Data.json`

## ⚙️ Metodologia

A análise foi conduzida em um notebook Jupyter (`telecomX_BR.ipynb`) e seguiu as seguintes etapas:

1.  **Extração e Transformação:** Os dados foram carregados, normalizados de uma estrutura JSON aninhada para um DataFrame tabular e tiveram seus tipos de dados corrigidos.
2.  **Limpeza de Dados:** Foram tratados valores ausentes e inconsistentes para garantir a qualidade e a precisão da análise.
3.  **Engenharia de Atributos (Feature Engineering):** Foram criadas novas variáveis (features) para aprofundar a análise, como o custo diário dos serviços (`account.Charges.Daily`), a quantidade de serviços adicionais contratados (`NumAddonServices`) e a categorização do tempo de contrato (`customer.tenure2`).
4.  **Análise Exploratória de Dados (EDA):** Utilizando bibliotecas de visualização de dados, foram criados diversos gráficos para explorar a relação entre as variáveis e a evasão de clientes, permitindo a identificação de tendências e padrões.

## 💡 Principais Descobertas (Insights)

A análise revelou um perfil claro do cliente com maior propensão à evasão. Os fatores mais determinantes são:

-   **Tipo de Contrato:** Clientes com **contratos mensais** apresentam uma taxa de churn drasticamente maior em comparação com aqueles em contratos anuais ou bianuais.
-   **Tempo de Contrato (Tenure):** Clientes **novos (com até 12 meses de serviço)** são muito mais propensos a cancelar. A lealdade aumenta significativamente com o tempo.
-   **Serviços Adicionais:** Clientes com **poucos ou nenhum serviço adicional** contratado tendem a evadir mais. A integração ao ecossistema de serviços da empresa funciona como um fator de retenção.
-   **Tipo de Serviço de Internet:** Clientes com serviço de **Fibra Óptica** apresentaram uma taxa de evasão maior, sugerindo possíveis problemas de preço, qualidade ou concorrência para este serviço específico.

## 🛠️ Tecnologias Utilizadas

-   **Linguagem:** Python 3
-   **Bibliotecas:**
    -   Pandas
    -   NumPy
    -   Matplotlib
    -   Seaborn
-   **Ambiente:** Google Colaboratory

## ✍️ Autor

**[Lucas Santos]**

-   **LinkedIn:** [https://linkedin.com/in/seu-linkedin](https://www.linkedin.com/in/lucassantos07)

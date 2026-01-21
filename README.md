# desafio-santander-etl-python
Pipeline ETL – Desafio Santander 2025 – Ciência de Dados com Python

# ETL de Leitos Hospitalares COVID-19

Este projeto implementa um pipeline **ETL (Extract, Transform, Load)** para coletar dados da API de Dados Abertos do Ministério da Saúde sobre ocupação hospitalar de leitos de estabelecimentos hospitalares, 

## 🚀 Passo a passo

### 1. Extração
- Utiliza a biblioteca `requests` para acessar a API.
- Converte o JSON retornado em um DataFrame Pandas.

### 2. Transformação
- Seleção e renomeação de colunas.
- Conversão de tipos (`float`, `boolean`, `datetime`).
- Criação da métrica `tx_leitos` (percentual de leitos SUS sobre o total hospitalar).

### 3. Carga
- Exporta os dados tratados para um arquivo CSV (`leitos_hospitalares.csv`).

## 📂 Estrutura do projeto
- `etl_leitos_hospitalares.ipynb` → Notebook com todo o passo a passo.
- `README.md` → Documentação do projeto.
- `leitos_hospitalares.csv` → Arquivo final gerado (opcional).

## 🛠️ Tecnologias utilizadas
- Python 3
- Pandas
- Requests

## 📊 Exemplo de saída
| ds_regiao | sg_unidade_federacao | ds_municipio | nm_hospital | qt_leitos_hospitalares | qt_leitos_sus | tx_leitos |
|-----------|-----------------------|--------------|-------------|------------------------|---------------|-----------|
| Sudeste   | MG                    | Paraguaçu    | Hospital X  | 100                    | 80            | 80.00%    |

---

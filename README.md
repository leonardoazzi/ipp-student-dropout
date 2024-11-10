# Predição de desistência acadêmica no Instituto Politécnico de Portalegre

Spot-checking ...

## Setup

1. Ambiente virtual
Crie um ambiente virtual para isolar os pacotes pip. Não seja um beta. Exemplo de criação de um ambiente chamado 'env':

```bash
python3 -m venv env
source env/bin/activate
```

2. Carregamento dos dados

O carregamento dos dados está sendo feito no EDA.ipynb através de cURL. Adaptar caminhos para outros sistemas operacionais, caso você for um beta.

- Linux (Sigma):
```bash
curl -L -o ./data/student-dropout.zip 'https://www.kaggle.com/api/v1/datasets/download/thedevastator/higher-education-predictors-of-student-retention'
unzip ./data/student-dropout.zip -d ./data
```
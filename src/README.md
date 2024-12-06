# Predição de evasão acadêmica no Instituto Politécnico de Portalegre 🇵🇹

Este trabalho tem como objetivo desenvolver um modelo baseado em Aprendizado de Máquina para prever a evasão acadêmica dos estudantes, ou seja,  se o aluno irá desistir, ou permanecer matriculado e se formar. A predição antecipada da situação acadêmica permite que as instituições de ensino superior adotem medidas proativas para apoiar os estudantes em risco e aprimorar as políticas educacionais.

![image](./IPP-Portalegre.jpg)

Utilizou-se o conjunto de dados ["Predicting Student Dropout and Academic Success"](https://doi.org/10.3390/data7110146), publicado em 2022. Este dataset abrange um amplo espectro de informações sobre alunos matriculados em diversos cursos de graduação do Instituto Politécnico de Portalegre, uma instituição de ensino superior em Portugal. Ele é composto por dados demográficos dos estudantes, fatores socioeconômicos e variáveis de desempenho acadêmico, coletados no momento da matrícula. Estes incluem o modo de aplicação, estado civil, curso escolhido, entre outros. Fatores macroeconômicos externos como a taxa de desemprego, taxa de inflação e o PIB da região também estão disponíveis, oferecendo dados adicionais que podem ser utilizados para entender contextos mais amplos que afetam os estudantes. Adicionalmente, o conjunto de dados permite a análise do desempenho estudantil ao término de dois semestres através de métricas sobre unidades curriculares creditadas, inscritas, avaliadas e aprovadas, bem como as notas correspondentes. Além desses dados, o dataset contém a situação do aluno no curso, já rotulado como “alvo” preditivo: graduado, desistente ou matriculado. 

## Setup

1. Ambiente virtual

Crie um ambiente virtual para isolar os pacotes pip. Exemplo de criação de um ambiente chamado 'env':

```bash
python3 -m venv env
source env/bin/activate # On macOS/Linux
.\venv\Scripts\activate # On Windows
```

2. Instalação dos pacotes pip
   
```bash
pip install -r requirements.txt
```

3. Carregamento dos dados

O carregamento dos dados está sendo feito no EDA.ipynb através de cURL. Adapte os caminhos para outros sistemas operacionais.

- Linux:

```bash
curl -L -o ./data/student-dropout.zip 'https://www.kaggle.com/api/v1/datasets/download/thedevastator/higher-education-predictors-of-student-retention'
unzip ./data/student-dropout.zip -d ./data
```

---
Autores: Leonardo Azzi Martins e Matheus Henrique Sabadin

INF01017 - Aprendizado de Máquina, Profa. Mariana Recamonde-Mendonza, 2024/2

Instituto de Informática – Universidade Federal do Rio Grande do Sul (UFRGS) 
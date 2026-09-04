# Projeto de Ciência de Dados: Eficiência do Sono

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Análise%20de%20dados-150458?logo=pandas)](https://pandas.pydata.org/)
[![Abrir EDA no Colab](https://img.shields.io/badge/Abrir%20EDA-Google%20Colab-F9AB00?logo=googlecolab&logoColor=white)](https://colab.research.google.com/github/NetoCassimiro/analise-eficiencia-do-sono/blob/main/An%C3%A1lise%20Explorat%C3%B3ria%20de%20Dados.ipynb)

[![Abrir Modelos no Colab](https://img.shields.io/badge/Abrir%20Modelos-Google%20Colab-F9AB00?logo=googlecolab&logoColor=white)](https://colab.research.google.com/github/NetoCassimiro/analise-eficiencia-do-sono/blob/main/An%C3%A1lise%20Comparativa%20de%20Modelos.ipynb)

Projeto autoral de Ciência de Dados desenvolvido durante o Bootcamp de Ciência de Dados da Atlântico Avanti. O trabalho abrange análise exploratória, preparação dos dados e comparação de modelos de regressão para investigar fatores associados e estimar a eficiência do sono.

> Os resultados representam associações observadas na amostra e não permitem estabelecer relações de causa e efeito.

## Etapas do projeto

- **Entrega #01 — Análise exploratória de dados:** concluída e disponível neste repositório.
- **Entrega #02 — Análise comparativa de modelos:** concluída, com pré-processamento em pipelines, validação cruzada e comparação de cinco modelos de regressão.

## Visão geral

O conjunto de dados possui **452 registros e 15 variáveis**, abrangendo:

- dados demográficos;
- horários e duração do sono;
- eficiência e fases do sono;
- número de despertares;
- hábitos como exercícios, tabagismo e consumo registrado de cafeína e álcool.

A análise exploratória foi organizada em quatro etapas:

1. descrição, qualidade e tratamento dos dados;
2. análise univariada das variáveis quantitativas, qualitativas e temporais;
3. análise bivariada, correlações e comparações por grupos;
4. análise multivariada de hábitos e características do sono.

Na etapa de modelagem, foram comparados o DummyRegressor, a Regressão Linear, o kNN, o SVR e o Random Forest por meio de validação cruzada k-fold com cinco divisões.


## Principais resultados

- A eficiência média do sono foi de aproximadamente **79%**.
- A porcentagem de sono leve apresentou forte correlação negativa com a eficiência (**r = -0,82**).
- A porcentagem de sono profundo apresentou forte correlação positiva com a eficiência (**r = 0,79**).
- O número de despertares apresentou correlação negativa moderada com a eficiência (**r = -0,56**).
- A duração do sono apresentou correlação próxima de zero com a eficiência (**r = -0,03**).
- Não foram observadas diferenças relevantes entre os gêneros.
- Na amostra, não fumantes apresentaram eficiência média de **81,7%**, enquanto fumantes apresentaram **73,4%**.
- A análise multivariada indicou que sono profundo, despertares e hábito de fumar estão conjuntamente associados à eficiência do sono.
- Na comparação entre cinco modelos de regressão, o **Random Forest** apresentou o melhor desempenho.
- O modelo obteve **MAE de 3,91 pontos percentuais**, **RMSE de 5,12 pontos percentuais** e **R² médio de 85,1%**, reduzindo o MAE em aproximadamente **65,7%** em relação ao baseline.

## Tecnologias e competências demonstradas

- Python
- Pandas e NumPy
- Matplotlib e Seaborn
- Scikit-learn
- limpeza, validação e preparação de dados
- análise exploratória e visualização de dados
- pipelines de pré-processamento
- regressão e Machine Learning
- validação cruzada k-fold
- avaliação com MAE, RMSE e R²
- análise de resíduos
- comunicação de resultados e limitações

## Estrutura do repositório

```text
.
├── apresentacao/
│   └── Eraldo_Cassimiro_DemoDay_Eficiencia_do_Sono.pdf
├── Análise Exploratória de Dados.ipynb
├── Análise Comparativa de Modelos.ipynb
├── Sleep_Efficiency.csv
├── README.md
└── requirements.txt
```

## Como executar

### Google Colab

1. Abra a **Entrega #01** pelo botão **Abrir EDA no Colab**, disponível no início deste README.
2. Execute as células em ordem e selecione o arquivo `Sleep_Efficiency.csv` quando solicitado.
3. Depois, abra a **Entrega #02** pelo botão **Abrir Modelos no Colab**.
4. Execute novamente as células em ordem e selecione o arquivo `Sleep_Efficiency.csv` quando solicitado.


### Ambiente local

```bash
git clone https://github.com/NetoCassimiro/analise-eficiencia-do-sono.git
cd analise-eficiencia-do-sono
python -m venv .venv
```

Ative o ambiente virtual e instale as dependências:

```bash
pip install -r requirements.txt
jupyter notebook
```

Os notebooks foram preparados para execução no Google Colab. Em um ambiente Jupyter local, substitua as células de upload pela leitura direta do arquivo:


```python
df = pd.read_csv("Sleep_Efficiency.csv")
```

## Dados

O conjunto de dados utilizado é o [Sleep Efficiency Dataset, disponibilizado no Kaggle](https://www.kaggle.com/datasets/equilibriumm/sleep-efficiency). Os dados são mantidos sem alterações no arquivo CSV; as conversões e os tratamentos necessários são documentados nos notebooks.

Consulte a página original para conhecer os termos aplicáveis à reutilização do conjunto de dados.

Projeto acadêmico desenvolvido por **Eraldo Cassimiro**.

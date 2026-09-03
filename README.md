# Projeto de Ciência de Dados: Eficiência do Sono

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Análise%20de%20dados-150458?logo=pandas)](https://pandas.pydata.org/)
[![Google Colab](https://img.shields.io/badge/Abrir-Google%20Colab-F9AB00?logo=googlecolab&logoColor=white)](https://colab.research.google.com/github/NetoCassimiro/analise-eficiencia-do-sono/blob/main/Squad01_Analise_Exploratoria_Sleep_Efficiency.ipynb)

Projeto de análise exploratória de dados desenvolvido no Bootcamp de Ciência de Dados da Avanti. O objetivo é compreender a distribuição dos hábitos e das características do sono e investigar fatores associados à eficiência do sono.

> Os resultados representam associações observadas na amostra e não permitem estabelecer relações de causa e efeito.

## Etapas do projeto

- **Entrega #00 — Identidade da equipe/autor:** definição do nome e da identidade visual do Squad-01.
- **Entrega #01 — Análise exploratória de dados:** concluída e disponível neste repositório.
- **Entrega #02 — Análise comparativa de modelos:** próxima etapa, que incluirá pré-processamento, validação, modelagem, comparação e discussão dos resultados.

## Visão geral

O conjunto de dados possui **452 registros e 15 variáveis**, abrangendo:

- dados demográficos;
- horários e duração do sono;
- eficiência e fases do sono;
- número de despertares;
- hábitos como exercícios, tabagismo e consumo registrado de cafeína e álcool.

A análise foi organizada em quatro etapas:

1. descrição, qualidade e tratamento dos dados;
2. análise univariada das variáveis quantitativas, qualitativas e temporais;
3. análise bivariada, correlações e comparações por grupos;
4. análise multivariada de hábitos e características do sono.

## Principais resultados

- A eficiência média do sono foi de aproximadamente **79%**.
- A porcentagem de sono leve apresentou forte correlação negativa com a eficiência (**r = -0,82**).
- A porcentagem de sono profundo apresentou forte correlação positiva com a eficiência (**r = 0,79**).
- O número de despertares apresentou correlação negativa moderada com a eficiência (**r = -0,56**).
- A duração do sono apresentou correlação próxima de zero com a eficiência (**r = -0,03**).
- Não foram observadas diferenças relevantes entre os gêneros.
- Na amostra, não fumantes apresentaram eficiência média de **81,7%**, enquanto fumantes apresentaram **73,4%**.
- A análise multivariada indicou que sono profundo, despertares e hábito de fumar estão conjuntamente associados à eficiência do sono.

## Tecnologias e competências demonstradas

- Python
- Pandas e NumPy
- Matplotlib e Seaborn
- limpeza e validação de dados
- tratamento de datas e horários
- estatística descritiva
- visualização de dados
- correlação de Pearson
- análises univariada, bivariada e multivariada
- comunicação de resultados e limitações

## Estrutura do repositório

```text
.
├── Sleep_Efficiency.csv
├── Squad01_Analise_Exploratoria_Sleep_Efficiency.ipynb
├── README.md
└── requirements.txt
```

## Como executar

### Google Colab

1. Abra o notebook pelo botão do Google Colab no início deste README.
2. Execute as células em ordem.
3. Quando a célula de upload for executada, selecione o arquivo `Sleep_Efficiency.csv`.

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

O notebook foi preparado para execução no Google Colab. Em um ambiente Jupyter local, substitua a célula de upload por:

```python
df = pd.read_csv("Sleep_Efficiency.csv")
```

## Dados

O conjunto de dados utilizado é o [Sleep Efficiency Dataset, disponibilizado no Kaggle](https://www.kaggle.com/datasets/equilibriumm/sleep-efficiency). Os dados são mantidos sem alterações no arquivo CSV; as conversões e os tratamentos necessários são documentados no notebook.

Consulte a página original para conhecer os termos aplicáveis à reutilização do conjunto de dados.

## Equipe

Projeto acadêmico desenvolvido por **Eraldo Cassimiro**.

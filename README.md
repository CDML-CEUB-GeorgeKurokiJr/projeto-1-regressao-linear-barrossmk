# Predição do Consumo de Combustível - Regressão Linear

## Objetivo

Este projeto tem como objetivo desenvolver um modelo de **Regressão Linear** capaz de prever o consumo de combustível de veículos (MPG - *Miles Per Gallon*) a partir de suas características técnicas. O projeto foi desenvolvido como atividade prática da disciplina de Deep Learning, aplicando conceitos fundamentais de pré-processamento de dados, treinamento e avaliação de modelos de regressão.


## Dataset

Foi utilizado o **Auto MPG Dataset**, um conjunto de dados amplamente utilizado em estudos de aprendizado de máquina para problemas de regressão.

O dataset possui **398 registros** e contém informações como:

- Número de cilindros;
- Cilindrada do motor;
- Potência (Horsepower);
- Peso do veículo;
- Aceleração;
- Ano do modelo;
- País de origem.

A variável **MPG** foi utilizada como variável alvo, representando o consumo de combustível dos veículos.


## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn


## Etapas do projeto

O desenvolvimento foi dividido nas seguintes etapas:

1. Importação das bibliotecas necessárias;
2. Carregamento do dataset;
3. Análise exploratória dos dados;
4. Tratamento dos valores ausentes e preparação dos dados;
5. Separação entre variáveis de entrada (X) e variável alvo (y);
6. Divisão dos dados em conjuntos de treinamento e teste;
7. Treinamento do modelo de Regressão Linear;
8. Realização das previsões;
9. Avaliação do desempenho do modelo;
10. Análise dos resultados obtidos.

Durante o pré-processamento foram removidos os registros com valores ausentes, descartada a coluna `name` e convertida a variável categórica `origin` em variáveis dummy para permitir seu uso pelo modelo.


## Resultados

O modelo apresentou os seguintes resultados no conjunto de teste:

| Métrica | Valor |
|---------|------:|
| MAE | 2.46 |
| MSE | 10.60 |
| RMSE | 3.26 |
| R² | 0.7923 |

O coeficiente de determinação (**R² = 0.7923**) indica que aproximadamente **79% da variação** do consumo de combustível foi explicada pelo modelo. Além disso, os valores obtidos para MAE e RMSE demonstram que as previsões ficaram relativamente próximas dos valores reais, indicando um desempenho satisfatório para este conjunto de dados.


## Como executar

1. Clone este repositório ou faça o download dos arquivos.
2. Instale as dependências necessárias:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

3. Abra o notebook Jupyter.
4. Execute as células em ordem para reproduzir todo o processo de treinamento e avaliação do modelo.


## Conclusão

Neste projeto foi possível aplicar todas as etapas básicas de um fluxo de aprendizado supervisionado utilizando Regressão Linear. Desde a exploração e preparação dos dados até a avaliação do modelo, foi demonstrado como as características dos veículos podem ser utilizadas para estimar seu consumo de combustível.

Os resultados obtidos mostram que a Regressão Linear é capaz de modelar boa parte da relação entre as variáveis do dataset, servindo como uma boa introdução aos modelos preditivos utilizados em Ciência de Dados e Deep Learning.

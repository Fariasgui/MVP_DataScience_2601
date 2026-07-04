# MVP Machine Learning & Analytics — Predição de Batalhas Pokémon

Este repositório contém o MVP desenvolvido para a disciplina de **Machine Learning & Analytics**, com o objetivo de construir um modelo preditivo capaz de estimar o vencedor de batalhas Pokémon a partir das características dos competidores.

O projeto utiliza o dataset **Pokémon Challenge**, disponível no Kaggle, composto por informações sobre atributos dos Pokémon e registros históricos de batalhas. A partir desses dados, foi construída uma base analítica para modelagem, incluindo etapas de preparação dos dados, engenharia de atributos, análise exploratória, treinamento de modelos, otimização de hiperparâmetros e avaliação final.

## Acesso ao Notebook

O notebook completo do MVP pode ser acessado pelo Google Colab no link abaixo:

[👉 Abrir MVP no Google Colab](https://colab.research.google.com/drive/1SAdtyl4o-p9HPuYnNIXzS2k79gGimhFQ?usp=sharing)

## Objetivo do Projeto

O objetivo deste MVP é aplicar técnicas de Machine Learning supervisionado para resolver um problema de classificação binária: prever se o primeiro Pokémon listado em uma batalha será o vencedor.

A variável alvo foi definida da seguinte forma:

- `1`: o primeiro Pokémon venceu;
- `0`: o segundo Pokémon venceu.

## Dataset Utilizado

O projeto utiliza o dataset **Pokémon Challenge**, que contém três arquivos principais:

- `pokemon.csv`: atributos dos Pokémon;
- `combats.csv`: histórico de batalhas com o vencedor conhecido;
- `tests.csv`: batalhas sem vencedor informado.

## Principais Etapas do MVP

O notebook está estruturado nas seguintes etapas:

1. Definição do problema;
2. Descrição e carregamento dos dados;
3. Construção da base analítica;
4. Análise exploratória dos dados;
5. Preparação dos dados e divisão treino/teste;
6. Criação de pipeline de pré-processamento;
7. Treinamento e comparação de modelos;
8. Otimização de hiperparâmetros;
9. Avaliação final no conjunto de teste;
10. Registro de boas práticas e rastreabilidade;
11. Conclusão do projeto.

## Modelos Avaliados

Foram avaliados diferentes algoritmos de classificação supervisionada:

- Regressão Logística, utilizada como baseline;
- Decision Tree;
- Random Forest;
- Gradient Boosting;
- Gradient Boosting otimizado.

O modelo final selecionado foi o **Gradient Boosting otimizado**, por apresentar o melhor desempenho geral e boa capacidade de generalização no conjunto de teste.

## Principais Técnicas Utilizadas

- Engenharia de atributos baseada nas diferenças entre os Pokémon;
- Tratamento de variáveis numéricas e categóricas;
- One-Hot Encoding;
- Padronização de variáveis numéricas;
- Pipeline com Scikit-Learn;
- Validação cruzada;
- Otimização com RandomizedSearchCV;
- Avaliação com Accuracy, Precision, Recall e F1-Score.

## Limitações

O modelo foi construído utilizando apenas os dados disponíveis no dataset original. Portanto, não foram consideradas informações adicionais relevantes do universo Pokémon, como:

- golpes utilizados;
- habilidades;
- itens equipados;
- vantagens e desvantagens entre tipos;
- condições específicas das batalhas.

## Autor

**Guilherme Farias**

MVP desenvolvido como parte da disciplina de Machine Learning & Analytics.

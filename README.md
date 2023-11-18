# Predição de Admissão com Rede Neural

## Visão Geral

Este projeto tem como objetivo prever a chance de admissão de estudantes usando uma rede neural. O conjunto de dados utilizado para treinamento e teste foi obtido do Kaggle: [Dataset de Admissão em Pós-Graduação](https://www.kaggle.com/mohansacharya/graduate-admissions).

## Informações do Arquivo

- **Arquivo:** neural_admission.ipynb
- **Fonte Original:** [Google Colab](https://colab.research.google.com/drive/1pY_FrW-6XELMj46Cx0DB0sUghrLUvAIV)

## Dependências

- pandas
- keras
- scikit-learn
- matplotlib

## Explicação do Código

O notebook segue as seguintes etapas principais:

### Carregamento e Pré-processamento dos Dados:

- Lê o conjunto de dados do Kaggle.
- Remove a coluna 'Serial No.'.
- Divide os dados em características de entrada (`x`) e variável alvo (`y`).

### Divisão dos Dados:

- Divide os dados em conjuntos de treinamento e teste usando uma proporção de 70-30.

### Criação do Modelo:

- Constrói um modelo de rede neural usando a API Sequencial do Keras.
- Utiliza o otimizador Adam para treinar o modelo.

### Treinamento e Avaliação:

- Treina o modelo usando os dados de treinamento.
- Plota o Erro Médio Absoluto (MAE) para os conjuntos de treinamento e teste ao longo das épocas.

### Otimizador RMSprop:

- Reutiliza a arquitetura do modelo com o otimizador RMSprop para comparação.
- Treina o modelo e plota o MAE.

### Avaliação do Modelo:

- Avalia a precisão do modelo (MAE) no conjunto de teste para os otimizadores Adam e RMSprop.

## Resultados

O notebook conclui com a avaliação do desempenho do modelo usando o Erro Médio Absoluto no conjunto de teste para os otimizadores Adam e RMSprop.

Sinta-se à vontade para explorar e modificar o notebook para experimentações adicionais.

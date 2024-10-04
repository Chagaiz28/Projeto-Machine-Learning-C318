# Projeto de Recomendação de Filmes

## Descrição

Este projeto foi desenvolvido para a matéria **C318 - Tópicos Especiais 2** e tem como objetivo criar um sistema de recomendação de filmes utilizando o dataset MovieLens. O sistema utiliza técnicas de filtragem colaborativa para recomendar filmes a usuários com base em suas avaliações anteriores.

## Estrutura do Projeto

O projeto é composto pelos seguintes arquivos:

- `PROJETOr.py`: Script principal que realiza a leitura dos dados, treinamento dos modelos de recomendação e geração de recomendações.
- `ml-32m`: Pasta contendo os datasets do MovieLens.
- `MD5`: Arquivo contendo os checksums MD5 para verificar a integridade dos arquivos CSV.

## Funcionalidades

1. **Carregamento e Verificação dos Dados**:
   - Os dados são carregados a partir dos arquivos CSV extraídos do arquivo `ml-32m.zip`.
   - A integridade dos arquivos é verificada utilizando checksums MD5.

2. **Exploração dos Dados**:
   - Exibição das primeiras linhas dos dados para exploração.
   - Visualização da distribuição das avaliações dos filmes.

3. **Criação da Matriz de Usuário-Item**:
   - Criação de uma matriz onde as linhas representam usuários e as colunas representam filmes, preenchida com as avaliações dos usuários.

4. **Treinamento de Modelos de Recomendação**:
   - Treinamento de dois modelos de recomendação: SVD (Singular Value Decomposition) e KNNBasic (K-Nearest Neighbors).
   - Avaliação dos modelos utilizando validação cruzada.

5. **Geração de Recomendações**:
   - Previsão de avaliações para um usuário específico e um filme específico.
   - Geração de recomendações de filmes para um usuário específico.

6. **Visualização das Recomendações**:
   - Visualização das recomendações de filmes em um gráfico de barras.

## Como Executar

### Pré-requisitos

Certifique-se de ter o Python e as seguintes bibliotecas instaladas:

- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-surprise`
- `hashlib`

Você pode instalar as bibliotecas necessárias usando o seguinte comando:

```sh
pip install pandas matplotlib seaborn scikit-surprise

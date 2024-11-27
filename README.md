# Projeto de Reconhecimento de Atividades Humanas (UCI HAR Dataset)

Este projeto tem como objetivo aplicar técnicas de **Reconhecimento de Atividades Humanas (HAR)** utilizando o conjunto de dados **UCI HAR Dataset**. O foco do projeto foi usar o algoritmo de **K-means clustering** para identificar e agrupar padrões de atividade humana a partir de dados de sensores.

## Índice

1. [Objetivo](#objetivo)
2. [Metodologia](#metodologia)
   - [Análise Exploratória](#análise-exploratória)
   - [K-means Clustering](#k-means-clustering)
3. [Resultados](#resultados)
4. [Instalação e Execução](#instalação-e-execução)
5. [Conclusão e Trabalhos Futuros](#conclusão-e-trabalhos-futuros)
6. [Referências](#referências)

## Objetivo

O objetivo deste projeto é explorar e analisar o **UCI HAR Dataset**, que contém dados de sensores coletados durante atividades humanas. O objetivo final é aplicar técnicas de **aprendizado de máquina não supervisionado** para **identificar padrões de atividade** utilizando o algoritmo de clustering **K-means**.

## Metodologia

A metodologia do projeto foi dividida em três etapas principais: **Análise Exploratória dos Dados**, **Implementação do K-means** e **Avaliação dos Resultados**.

### Análise Exploratória

A análise exploratória dos dados incluiu:
- Carregamento e limpeza dos dados.
- Análise das variáveis presentes no conjunto de dados (sensor data).
- Geração de uma matriz de correlação para entender as relações entre as variáveis.
- Visualização dos dados utilizando PCA (Análise de Componentes Principais) para reduzir a dimensionalidade e facilitar a análise.

### K-means Clustering

O algoritmo **K-means** foi utilizado para segmentar os dados em clusters. O número de clusters foi determinado utilizando o método do cotovelo e a avaliação do **Silhouette Score**. As etapas incluem:
- Normalização dos dados com o **StandardScaler**.
- Aplicação do K-means com diferentes valores de K (número de clusters).
- Avaliação da qualidade dos clusters com o **Silhouette Score**.

## Resultados

Os principais resultados incluem:
- A análise PCA mostrou que os dois primeiros componentes explicam aproximadamente **57% da variância** nos dados.
- O método do cotovelo e o Silhouette Score indicaram que o número ideal de clusters é **4**.
- Visualizações de clustering foram geradas utilizando PCA para projetar os dados em 2D.

### Gráficos

Abaixo, seguem alguns dos gráficos gerados durante a análise do projeto:

1. **Mapa de Correlação**
   
   ![Mapa de Correlação](./assets/correlation_heatmap.png)
   
2. **PCA: Visualização das Atividades com 2 Componentes Principais**

   ![PCA](./assets/pca_visualization.png)

3. **Método do Cotovelo - Inércia dos Clusters**

   ![Método do Cotovelo](./assets/elbow_method.png)

4. **Silhouette Score por Número de Clusters**

   ![Silhouette Score](./assets/silhouette_score.png)

## Instalação e Execução

Para executar este projeto em sua máquina local, siga os passos abaixo:

### Pré-requisitos

- Python 3.x
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`

### Instalação

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/recognition-of-human-activities.git

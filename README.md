# Previsão de Evasão e Sucesso Acadêmico em Instituições de Ensino Superior com Random Forest
![Static Badge](https://img.shields.io/badge/Status-Finalizado-Green)

## Descrição

Este projeto utiliza aprendizado de máquina supervisionado para prever a evasão e o sucesso acadêmico de estudantes universitários com base em dados coletados no momento da matrícula. O modelo Random Forest Classifier é empregado para lidar com o desequilíbrio de classes e fornecer insights valiosos para intervenções direcionadas.

## Tecnologias Utilizadas

* **Linguagem de Programação:** Python
* **Bibliotecas de Aprendizado de Máquina:**
    * Scikit-learn (RandomForestClassifier, métricas de avaliação, etc.)
    * Imbalanced-learn (técnica de reamostragem SMOTE)
* **Bibliotecas de Manipulação de Dados:**
    * Pandas
* **Visualização de Dados:**
    * Matplotlib
    * Seaborn
    * Plotly

## Detalhes

### 1. Obtenção e Análise Exploratória dos dados

* **Fontes de Dados:** Os dados utilizados foram obtidos a partir do [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/697/predict+students+dropout+and+academic+success)
* **Análise:**
    * Desenvolvida visualização gráfica de características relevantes dos dados.
    * Identificação dos atributos mais importantes para a previsão.
    * Análise do impacto de diferentes fatores na evasão e no sucesso acadêmico.
    * Analisada a distribuição da variável alvo e como ela poderia influenciar o modelo.

### 2. Implementação de OneHotEncoder

<img width="1006" alt="image" src="https://github.com/ledsouza/machine-learning-students-dropout/assets/56280624/d6e76116-7070-43cc-b5d9-dcd99290adff">

### 3. Modelagem Preditiva

* **Algoritmo:** Random Forest Classifier
    * Adequado para lidar com desequilíbrio de classes.
    * Adequado para lidar com multiclasses.
    * Robusto a outliers e ruído nos dados.
    * Interpretabilidade razoável.
* **Validação Cruzada:**
    * Garante a generalização do modelo para novos dados.
    * Permite ajuste de hiperparâmetros.
* **Métricas de Avaliação:**
    * Acurácia (com cautela devido ao desequilíbrio).
    * Precisão, recall, F1-score (para cada classe).
* **Técnicas de Reamostragem:**
    * Oversampling (SMOTE) para lidar com o desequilíbrio de classes.

<img width="560" alt="image" src="https://github.com/ledsouza/machine-learning-students-dropout/assets/56280624/14666977-bb04-4467-b8a7-ec1b81011232">

### Observações

* **Desequilíbrio de Classes:** É crucial abordar o desequilíbrio de classes para evitar que o modelo seja enviesado em favor da classe majoritária.
* **Interpretabilidade:** O Random Forest oferece alguma interpretabilidade, mas técnicas adicionais podem ser exploradas para entender melhor as decisões do modelo.

Este projeto tem o potencial de fornecer informações valiosas para as instituições de ensino superior, permitindo que elas identifiquem estudantes em risco de evasão ou com dificuldades acadêmicas e implementem intervenções direcionadas para melhorar seus resultados.

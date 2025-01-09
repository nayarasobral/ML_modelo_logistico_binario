# **Previsão de Cliques em Anúncios de Produtos Hospitalares**

Este projeto tem como objetivo criar um modelo de aprendizado de máquina para prever a probabilidade de cliques em anúncios patrocinados de produtos hospitalares, com base em características do usuário e informações sobre os anúncios. O modelo utiliza **Regressão Logística Binária**, uma técnica de classificação amplamente utilizada em problemas de marketing digital.

---

## **Objetivo do Projeto**
- Prever se um cliente clicará ou não em um anúncio, baseado em dados como demografia, comportamento e características do anúncio.
- Utilizar técnicas de **aprendizado supervisionado** para criar insights que podem ajudar a otimizar campanhas de marketing digital.

---

## **Estrutura do Projeto**

### **1. Análise do Problema e Configuração Inicial**
- Compreensão do problema de previsão de cliques.
- Configuração inicial do ambiente e importação das bibliotecas necessárias.

### **2. Pré-Processamento e Engenharia de Dados**
- Tratamento de valores ausentes.
- Codificação de variáveis categóricas (**One-Hot Encoding**).
- Normalização de variáveis numéricas.
- Divisão do conjunto de dados em treino e teste.

### **3. Treinamento e Avaliação Inicial do Modelo**
- Treinamento do modelo de **Regressão Logística**.
- Avaliação do desempenho usando métricas como:
  - **Acurácia**
  - **Precisão**
  - **Recall**
  - **F1-Score**
  - **Área sob a curva ROC (AUC-ROC)**

### **4. Interpretação e Ajustes no Modelo**
- Análise dos coeficientes do modelo para entender o impacto das variáveis.
- Ajuste de hiperparâmetros utilizando **GridSearchCV**.

---

## **Ferramentas e Tecnologias**
- **Python**
- **Bibliotecas:**
  - `pandas` - Manipulação e análise de dados.
  - `numpy` - Computação numérica.
  - `matplotlib` e `seaborn` - Visualização de dados.
  - `scikit-learn` - Construção e avaliação do modelo de machine learning.

---

## **Dataset**
Os dados utilizados neste projeto foram obtidos do Kaggle:  
📂 **[Online Ad Click Prediction Dataset](https://www.kaggle.com/datasets/natchananprabhong/online-ad-click-prediction-dataset?resource=download)**

### **Características do Dataset:**
- Variável dependente: `Clicked` (se o cliente clicou ou não no anúncio).
- Variáveis independentes incluem:
  - Dados demográficos do usuário.
  - Informações sobre o anúncio.
  - Comportamento anterior de navegação.

---

## **Resultados**
- **Modelo:** Regressão Logística
- **Métricas:**
  - **Acurácia:** 84%
  - **ROC-AUC:** 0.85
- **Variáveis Relevantes:**
  - **Tempo no site** (`Time_Spent_on_Site`): Clientes que passaram mais tempo no site têm maior probabilidade de clicar no anúncio.
  - **Número de páginas visualizadas** (`Number_of_Pages_Viewed`): Quanto mais páginas o cliente visualiza, maior a probabilidade de clicar.

---

## **Como Reproduzir o Projeto**

1. **Clone este repositório:**
   ```bash
   git clone https://github.com/SeuUsuario/ML_modelo_logistico_binario.git
   ```

2. **Instale as dependências:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Execute o notebook Jupyter:**
   Abra o arquivo `clicking.ipynb` e execute as células para reproduzir os resultados.

---

## **Próximos Passos**
- Explorar técnicas mais avançadas, como árvores de decisão e ensemble methods.
- Implementar o modelo em um ambiente web utilizando **Flask** ou **Streamlit** para previsões em tempo real.

---

## **Contribuições**
Contribuições são bem-vindas! Caso tenha sugestões ou encontre problemas, sinta-se à vontade para abrir uma **issue** ou criar um **pull request**.


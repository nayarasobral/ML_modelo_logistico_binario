# Projeto: Previsão de Cliques em Anúncios

Este projeto tem como objetivo criar um modelo de aprendizado de máquina para prever a probabilidade de cliques em anúncios, com base em características do usuário. O modelo foi implementado com ***Regressão Logística***.

---

## Estrutura do Projeto

1. **Análise do Problema e Configuração Inicial**:
   - Compreensão do problema de previsão de cliques.
   - Configuração inicial do ambiente e importação das bibliotecas necessárias.

2. **Pré-Processamento e Engenharia de Dados**:
   - Tratamento de valores ausentes.
   - Codificação de variáveis categóricas (One-Hot Encoding).
   - Normalização de variáveis numéricas.
   - Divisão do conjunto de dados em treino e teste.

3. **Treinamento e Avaliação Inicial do Modelo**:
   - Treinamento do modelo de Regressão Logística.
   - Avaliação do desempenho usando métricas como:
     - Acurácia
     - Precisão
     - Recall
     - F1-Score
     - Área sob a curva ROC (AUC-ROC).

4. **Interpretação e Ajustes no Modelo**:
   - Análise de coeficientes para identificar a relevância de cada variável.
   - Ajuste de hiperparâmetros usando GridSearchCV.
   - Reavaliação do modelo ajustado.

5. **Deploy Simples**:


---

## Como Executar o Projeto

### 1. Configuração do Ambiente

Certifique-se de que as seguintes bibliotecas estão instaladas:

pandas==1.5.2
numpy==1.21.0
scikit-learn==1.2.0
matplotlib==3.5.1
seaborn==0.11.2
joblib==1.2.0
imblearn==0.9.0
xgboost==1.6.2

Instale as dependências com o comando:

```bash
pip install -r requirements.txt
```

> **Nota:** Se o arquivo `requirements.txt` não estiver disponível, instale as bibliotecas individualmente usando `pip`.

---

### 2. Executando o Modelo

#### **Treinamento do Modelo**
Para treinar o modelo, execute o notebook Jupyter fornecido: `clicking.ipynb`. O notebook contém todas as etapas desde a análise inicial até o treinamento e avaliação do modelo.

---

## Resultados

- **Modelo**: Regressão Logística
- **Métricas**:
  - Acurácia: 84%
  - ROC-AUC: 0.85
- **Variáveis Relevantes**:
  - Tempo no site (`Time_Spent_on_Site`)
  - Número de páginas visualizadas (`Number_of_Pages_Viewed`)

---

## Estrutura do Projeto

ML_LOGISTIC_CLICK/
│
├── ads_clicking.csv           # Conjunto de dados usado para treinar e avaliar o modelo
├── clicking.ipynb             # Notebook Jupyter com o código completo do projeto
├── feature_columns.pkl        # Arquivo serializado com as colunas utilizadas no modelo
├── scaler.pkl                 # Arquivo serializado com o objeto StandardScaler usado na normalização
├── requirements.txt           # Lista de dependências do projeto
├── README.md                  # Documentação do projeto
└── Restart                    # (Indefinido, pode ser um marcador ou arquivo temporário)

```

---

## **Como Executar o Projeto**

1. **Clone o repositório**:
   ```bash
   git clone <link_do_repositorio>
   cd ML_LOGISTIC_CLICK
   ```

2. **Configure o ambiente virtual** (opcional, mas recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```

3. **Instale as dependências**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Abra o notebook**:
   Inicie o Jupyter Notebook e abra `clicking.ipynb`:
   ```bash
   jupyter notebook
   ```

5. **Execute as células no notebook**:
   Siga as etapas no notebook para carregar os dados, treinar o modelo, e realizar as previsões.

---

## **Contribuição**
Se você encontrar problemas ou quiser contribuir para melhorar o modelo, sinta-se à vontade para abrir uma issue ou enviar um pull request.

---

## **Licença**
Este projeto está sob a licença MIT. Sinta-se à vontade para usar e modificar.


Sinta-se à vontade para contribuir com melhorias ou abrir issues para discutir ideias!



# ML_modelo_logistico_binario

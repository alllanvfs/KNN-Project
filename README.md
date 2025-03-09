# 📌 Projeto de Classificação com K-Nearest Neighbors (KNN)

## 📖 Sobre o Projeto
Este projeto implementa um modelo de classificação utilizando o algoritmo **K-Nearest Neighbors (KNN)** para prever a presença de minas ou rochas com base em dados de ondas sonoras. A otimização do modelo foi realizada com **validação cruzada estratificada (StratifiedKFold)** e **Grid Search** para encontrar o melhor valor de `K`.

## 📊 Conjunto de Dados
O dataset utilizado foi **Sonar All-Data**, que contém **60 atributos numéricos** extraídos de sinais acústicos. As classes alvo são:
- **R (Rock)** → Representa rochas
- **M (Mine)** → Representa minas

Para facilitar a modelagem, os rótulos foram convertidos para valores numéricos:
- `R` → `0`
- `M` → `1`

## 🛠 Tecnologias Utilizadas
- Python
- Pandas & NumPy (manipulação de dados)
- Seaborn & Matplotlib (visualizações)
- Scikit-learn (modelagem e validação)

## 🚀 Implementação
### 1️⃣ Pré-processamento dos dados
- Carregamento do dataset
- Conversão de rótulos para valores numéricos
- Padronização das variáveis preditoras usando **StandardScaler**
- Divisão em conjuntos de treino e teste (**90% treino / 10% teste**)
- Verificação de desbalanceamento das classes

### 2️⃣ Construção do Modelo
- Utilização de **Pipeline** para aplicar a padronização e o modelo KNN
- Busca do melhor valor de `K` através do **GridSearchCV**
- Uso de **StratifiedKFold (k=5)** para garantir divisão equilibrada das classes

### 3️⃣ Avaliação do Modelo
- **Relatório de classificação (classification report)**
- **Matriz de confusão com heatmap**
- **Acurácia do modelo**

## 📌 Resultados Obtidos
O modelo apresentou um desempenho sólido na classificação das amostras, com um **melhor valor de `K` encontrado via Grid Search**. A matriz de confusão e as métricas de desempenho foram utilizadas para avaliar a eficácia do modelo.

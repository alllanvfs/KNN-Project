# 📌 K-Nearest Neighbors (KNN) Classification Project

## 📖 About the Project
This project implements a classification model using the **K-Nearest Neighbors (KNN)** algorithm to predict the presence of mines or rocks based on sound wave data. The model optimization was done using **Stratified Cross-Validation (StratifiedKFold)** and **Grid Search** to find the best value for `K`.

## 📊 Dataset
The dataset used was **Sonar All-Data**, which contains **60 numerical attributes** extracted from acoustic signals. The target classes are:
- **R (Rock)** → Represents rocks
- **M (Mine)** → Represents mines

To facilitate modeling, the labels were converted to numeric values:
- `R` → `0`
- `M` → `1`

## 🛠 Technologies Used
- Python
- Pandas & NumPy (data manipulation)
- Seaborn & Matplotlib (visualizations)
- Scikit-learn (modeling and validation)

## 🚀 Implementation
### 1️⃣ Data Preprocessing
- Loading the dataset
- Converting labels to numeric values
- Standardizing predictor variables using **StandardScaler**
- Splitting into training and testing sets (**90% training / 10% testing**)
- Checking for class imbalance

### 2️⃣ Model Construction
- Using **Pipeline** to apply standardization and the KNN model
- Searching for the best value of `K` through **GridSearchCV**
- Using **StratifiedKFold (k=5)** to ensure balanced class division

### 3️⃣ Model Evaluation
- **Classification report**
- **Confusion matrix with heatmap**
- **Model accuracy**

## 📌 Results
The model showed solid performance in classifying samples, with the **best value for `K` found via Grid Search**. The confusion matrix and performance metrics were used to evaluate the model's effectiveness.

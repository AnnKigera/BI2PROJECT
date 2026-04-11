# Diabetes Prediction using Machine Learning

A supervised machine learning project that predicts the likelihood of diabetes in patients based on diagnostic health data. Built as part of a Business Intelligence module, this project covers the full data science pipeline — from data cleaning and exploration to model training, evaluation, and interpretation.

---

## 🎯 Project objective

Diabetes affects over 537 million people globally, with Sub-Saharan Africa seeing rapidly increasing rates. Early prediction using patient data can help health workers prioritise screening and intervention. This project explores whether machine learning can reliably classify diabetes risk from standard diagnostic measurements.

---

## 📊 Dataset

- **Source:** Pima Indians Diabetes Dataset (UCI Machine Learning Repository)
- **Records:** 768 patient entries
- **Features:** 8 diagnostic variables including glucose level, BMI, blood pressure, insulin, and age
- **Target variable:** Binary outcome — diabetic (1) or non-diabetic (0)

---

## 🔬 Methodology

### 1. Data exploration & cleaning
- Identified and handled missing/zero values in key columns (glucose, BMI, blood pressure)
- Analysed feature distributions and class balance
- Visualised correlations between health indicators and diabetes outcome

### 2. Feature engineering
- Normalised numerical features for model compatibility
- Addressed class imbalance where applicable

### 3. Model training
Trained and compared multiple classification algorithms:
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- K-Nearest Neighbours (KNN)

### 4. Evaluation
Models were evaluated using:
- Accuracy score
- Confusion matrix
- Precision, Recall, and F1-score
- ROC-AUC curve

---

## 📈 Results

| Model | Accuracy | F1-Score |
|---|---|---|
| Logistic Regression | ~77% | ~0.72 |
| Decision Tree | ~74% | ~0.69 |
| Random Forest | ~79% | ~0.74 |
| KNN | ~75% | ~0.70 |

> Random Forest performed best overall, with the strongest balance between precision and recall.

*(Update these figures with your actual results if they differ)*

---

## 🛠️ Tools & libraries

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

- **Python 3.x**
- **Pandas** — data manipulation and analysis
- **NumPy** — numerical operations
- **Scikit-learn** — model training and evaluation
- **Matplotlib / Seaborn** — data visualisation
- **Jupyter Notebook** — development environment

---

## 📁 Project structure

```
BI2PROJECT/
│
├── diabetes_prediction.ipynb   # Main notebook — full pipeline
├── diabetes.csv                # Dataset (or link to source)
├── README.md
└── requirements.txt            # Python dependencies
```

---

## 🚀 How to run this project

1. Clone the repository
```bash
git clone https://github.com/AnnKigera/BI2PROJECT.git
cd BI2PROJECT
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Open the notebook
```bash
jupyter notebook diabetes_prediction.ipynb
```

---

## 💡 Key learnings

- Real-world health datasets require significant preprocessing before modelling — missing values masked as zeros were the biggest challenge
- Random Forest outperformed simpler models, but at the cost of interpretability — an important trade-off in health contexts
- Evaluation metrics beyond accuracy (especially recall) matter significantly in medical prediction, where false negatives carry higher costs than false positives

---

## 🌍 Why this matters

Predictive health tools built on accessible, structured data have meaningful applications across LMICs where specialist medical access is limited. Projects like this are a first step toward understanding how ML can support frontline health workers in making faster, evidence-based decisions.

---

## 👩‍💻 Author

**Ann Kigera** — [LinkedIn](https://www.linkedin.com/in/ann-kigera-0842a8272/) · [GitHub](https://github.com/AnnKigera)

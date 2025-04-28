#  Stroke Risk Prediction Project

##  Project Overview
Stroke remains a leading cause of death and long-term disability worldwide.  
This project aims to develop a machine learning model that can predict the likelihood of an individual experiencing a stroke based on clinical and demographic health indicators.

Our goal is to support preventive healthcare initiatives by identifying high-risk individuals early using accessible patient data.

---

## 🛠️ Methods and Workflow

- **Data Wrangling**:  
  - Imputed missing values for BMI using median strategy.
  - Created dummy/indicator features for categorical variables.
  - Standardized magnitude of numeric features.
  
- **Exploratory Data Analysis (EDA)**:  
  - Analyzed distributions of age, BMI, glucose levels.
  - Examined relationships between health indicators and stroke occurrence.
  - Visualized feature correlations.

- **Modeling**:  
  - Built Logistic Regression, Random Forest, and Support Vector Machine (SVM) models.
  - Applied hyperparameter tuning using GridSearchCV.
  - Evaluated models using Accuracy, Recall, Precision, F1-Score, and ROC AUC metrics.

- **Interpretability**:  
  - Used SHAP (SHapley Additive exPlanations) to interpret feature importance for model transparency.

- **Learning Curve Analysis**:  
  - Assessed model learning behavior to check for overfitting/underfitting.

---

##  Results

| Model                     | Accuracy | Recall (Stroke) | Precision (Stroke) | F1 Score (Stroke) | ROC AUC |
|----------------------------|:--------:|:---------------:|:------------------:|:-----------------:|:-------:|
| Logistic Regression        |   0.74   |      0.76       |        0.13         |       0.22        |  0.84   |
| Random Forest (Tuned)      |   0.87   |      0.31       |        0.14         |       0.19        |  0.92   |
| SVM (Tuned)                |   0.71   |      0.73       |        0.11         |       0.20        |  0.81   |

 **Final Model Selected**:  
**Random Forest Classifier (Tuned)** — achieving 87% accuracy and a 92% ROC AUC score.

---

##  Key Insights

- **Top predictors** of stroke risk: Age, Average Glucose Level, Heart Disease status.
- **Preventive strategies** could prioritize elderly individuals and those with chronic conditions like hypertension and diabetes.
- **Class imbalance** (few stroke cases) remains a challenge for optimizing recall without harming precision.

---

## Technologies Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- SHAP
- Jupyter Notebook

---

##  Repository Structure


##  Author

**Manuel Ramirez Chimarro**  
Data Science Career Track – Springboard


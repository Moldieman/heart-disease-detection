# Heart Disease Detection using Machine Learning

## CSCA5622: Introduction to Machine Learning – Final Project (Supervised Learning)

This repository explores the application of supervised learning algorithms to predict the likelihood of heart disease in individuals using the well-known UCI Heart Disease dataset.

---

## Project Summary

Heart disease continues to be a major global health concern. The purpose of this project is to:
1. Build an effective predictive model for identifying patients at risk of heart disease  
2. Evaluate and compare the performance of various machine learning algorithms  
3. Highlight which clinical and demographic features most strongly influence heart disease outcomes  

---

## Dataset Description

The dataset used is the **UCI Heart Disease dataset**, which aggregates clinical and demographic data from multiple sources, including the **Cleveland Clinic Foundation**.  

It includes attributes such as:
- Patient demographics (age, gender, etc.)  
- Clinical indicators (cholesterol, resting blood pressure, etc.)  
- Results from diagnostic tests (ECG, stress test outcomes, etc.)  
- The target variable: presence or absence of heart disease  

---

## Approach

The workflow for this project follows a standard end-to-end machine learning pipeline:

1. **Exploratory Data Analysis (EDA)**  
   - Examination of variable distributions and relationships  
   - Visualizations to identify trends and potential anomalies  
   - Statistical and correlation analysis  

2. **Data Preparation**  
   - Handling missing or inconsistent data  
   - Managing outliers  
   - Normalizing and encoding features  

3. **Feature Engineering**  
   - Creating new relevant features  
   - Selecting the most informative predictors  

4. **Model Building**  
   - Implementation of the following supervised models:  
     - Logistic Regression  
     - Random Forest Classifier  
     - Support Vector Machine (SVM)  
     - XGBoost  
   - Cross-validation for model robustness  
   - Hyperparameter optimization to improve accuracy  

5. **Performance Evaluation**  
   - Model comparison using multiple metrics  
   - ROC/AUC and confusion matrix analysis  
   - Feature importance interpretation  

---

## Results Summary

- The top-performing model reached an **accuracy of 85.53%** on the test dataset.  
- Features that had the strongest predictive power included **thal (thallium stress test results)**, **ca (number of major vessels)**, and **cp (type of chest pain)**.  
- The final model shows strong promise for assisting in early diagnosis and prevention strategies in healthcare settings.  

---

## Project Structure

heart-disease-detection/
├── data/
│ ├── raw/ # Contains the UCI dataset
├── models/ # Stores serialized trained models
├── heart_disease_analysis.ipynb # Jupyter notebook with analysis and results
├── README.md # Project documentation
└── requirements.txt # List of required Python packages

## Getting Started

1. **Clone the repository**
```bash
  git clone https://github.com/moldieman/heart-disease-detection.git
```

2. **Set up a virtual environment and install dependencies**
```bash
  python -m venv env
  source env/bin/activate
  pip install -r requirements.txt
```

3. ***Launch the notebook***
```bash
jupyter notebook heart_disease_analysis.ipynb
```

## Required Dependencies

- Python 3.8
- pandas
- numpy
- scikit-learn
- matplotlib
- xgboost
- seaborn

## Data Source

1. UCI Machine Learning Repository – Heart Disease Dataset
   https://archive.ics.uci.edu/dataset/45/heart+disease

## Author

Alexander Molde

## License

This project is licensed under the MIT License.
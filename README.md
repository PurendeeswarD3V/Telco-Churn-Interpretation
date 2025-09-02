# Telco-Churn-Interpretation 

A machine learning project to **predict and interpret customer churn** using **XGBoost, CatBoost, and LightGBM** on the Telco Customer Churn dataset.  
This project demonstrates model training, evaluation, and explainability with **SHAP values** and interactive visualizations.

---

##  Repository Structure

```bash
assignment-d3v/
│── data/
│   └── WA_Fn_UseC_-Telo-Customer-Churn.csv        # Raw dataset
│
│── models/
│   ├── cat_model.joblib                           # Trained CatBoost model
│   ├── lgbm_model.joblib                          # Trained LightGBM model
│   ├── xgb_model.joblib                           # Trained XGBoost model
│   └── preprocessor.joblib                        # Preprocessing pipeline
│
│── outputs/
│   ├── catboost_shap_values.csv                   # SHAP values for CatBoost
│   ├── xgb_shap_values.csv                        # SHAP values for XGBoost
│   └── plots/                                     # Generated plots & charts
│
│── notebooks/
│   └── Telco.ipynb                                # Main Jupyter notebook
│
│── requirements.txt                               # Python dependencies
│── README.md                                      # Project documentation


---

## ✨ Features

- **Data Preprocessing**  
  Handles categorical & numerical features using `scikit-learn` pipelines.  

- **Model Training**  
  Trains three ensemble models:  
  - XGBoost  
  - CatBoost  
  - LightGBM  

- **Explainability with SHAP**  
  - Global feature importance  
  - Local instance-level explanations  
  - Interactive plots  

- **Visualization**  
  - Precision-Recall curves  
  - ROC curves  
  - SHAP summary plots  

---

## ⚙️ Installation

Clone this repository:

```bash
git clone https://github.com/your-username/Telco-Churn-Interpretation.git
cd Telco-Churn-Interpretation



python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows

Install dependencies:


pip install -r requirements.txt

## Usage
Run the Jupyter notebook for training and interpretation:


jupyter notebook notebooks/Telco.ipynb
After execution:

Trained models are stored in models/

SHAP values and plots are stored in outputs/

## Results
XGBoost, CatBoost, and LightGBM achieve strong performance on churn prediction.

SHAP values reveal MonthlyCharges, Contract type, and Tenure as top drivers of churn.

Visualizations highlight both global importance and individual customer explanations.

## Tech Stack
Python 3.9+

XGBoost

CatBoost

LightGBM

Scikit-learn

SHAP

Matplotlib / Plotly

## License
This project is open-source and available under the MIT License.

## Acknowledgements
Dataset: Telco Customer Churn (Kaggle)
Inspiration from explainable AI and model interpretability best practices.

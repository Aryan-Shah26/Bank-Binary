# 🏦 Bank Binary Classification (Kaggle Competition)

This repository contains two versions of solution notebooks for the **Bank Binary Classification** problem from Kaggle.  
The challenge is a **binary classification** task where the objective is to predict whether a client is offered a loan or not based on demographic and campaign-related data.  

---

## 📂 Repository Contents
- **`bank-binary.ipynb`**  
  - Initial version of the solution  
  - Includes data preprocessing, EDA, SMOTE for handling imbalance  
  - Trains a LightGBM model and evaluates using ROC, AUC, and confusion matrix  

- **`bank-binary-version-2.ipynb`**  
  - Improved version with additional feature preprocessing and evaluation  
  - Uses **StandardScaler** for numerical features  
  - Includes cross-validation (KFold, StratifiedKFold)  
  - Evaluates multiple metrics: accuracy, precision, recall, f1-score, ROC AUC  
  - Trains a LightGBM model with hyperparameter tuning (`lgb_params`)  

---

## 📊 Competition Context
- **Platform**: Kaggle  
- **Task**: Predict a binary target variable (`y`):  
  - `1` → client is offered the loan
  - `0` → client is not offered the loan  
- **Dataset**: Provided via Kaggle competition (not included in this repository; must be downloaded separately).  

---

## ⚙️ Workflow

### Version 1
1. Load dataset with pandas  
2. Explore with matplotlib & seaborn  
3. Encode categorical variables with LabelEncoder  
4. Handle imbalance with SMOTE  
5. Train LightGBM classifier  
6. Evaluate with ROC curve, AUC, and confusion matrix  

### Version 2
1. Load and scale features with StandardScaler  
2. Encode categorical variables with LabelEncoder  
3. Apply KFold and StratifiedKFold cross-validation  
4. Train LightGBM with tuned parameters  
5. Evaluate using accuracy, precision, recall, f1-score, and ROC AUC  

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>

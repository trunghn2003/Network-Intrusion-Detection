#  Network Intrusion Detection System

A machine learning-based system for detecting network intrusions using the NSL-KDD dataset. The system implements and compares several models including Logistic Regression, Random Forest and Neural Networks, achieving up to **99.99% accuracy**.

---

## 📊 Dataset

### 🔹 Structure
The dataset contains 43 features, categorized as:

- **Basic features**: `duration`, `protocol_type`, `service`, `flag`
- **Traffic content features**: `src_bytes`, `dst_bytes`, `land`, `wrong_fragment`
- **Time-based traffic features**: `count`, `srv_count`
- **Host-based traffic features**: `dst_host_count`, `dst_host_srv_count`

### 🔹 Files
Ensure the following files are placed in the root project directory:

- `Train_data.csv` (86,845 records)
- `Test_data.csv` (21,712 records)

### 🔹 Target
- **Target Variable**: `attack`  
  - `0` = Normal  
  - `1` = Attack

---

##  Key Features

- 🧠 One-hot encoding for categorical variables
- 📏 Feature normalization using `StandardScaler`
- 📊 70-30 train-test split
- ✅ Evaluation using **ROC-AUC** and **accuracy**

---

## ⚙️ Models & Performance

| Model               | Accuracy | ROC-AUC |
|--------------------|----------|---------|
| Logistic Regression| 99.1%    | 0.992   |
| Random Forest      | 99.0%    | 0.500   |
| Neural Network     | 99.992%  | 0.999   |

> Note: XGBoost can also be included with further tuning for performance enhancement.

---
## How to run

- Execute the Jupyter notebook Hackathon2.ipynb

The code will:

- Load and preprocess data

- Train selected models

- Evaluate performance metrics

## 🧰 Requirements

- Python 3.8+
- Install dependencies:

```bash
pip install pandas numpy scikit-learn xgboost tensorflow

 

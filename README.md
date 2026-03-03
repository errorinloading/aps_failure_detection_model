
# APS Failure Detection using Machine Learning

## 📌 Overview

This project predicts failures in the Air Pressure System (APS) of Scania trucks using sensor data. The dataset is highly imbalanced, with failure cases being rare but costly. The objective is to minimize high-cost false negatives while maintaining strong recall.

---

## 📊 Dataset

**Source:** UCI Machine Learning Repository  
**Dataset:** APS Failure at Scania Trucks  

- ~60,000 samples  
- 171 sensor features  
- Target:  
  - `pos` → APS failure  
  - `neg` → No failure  
- Highly imbalanced dataset  
- Missing values represented as `na`

Dataset link:  
https://archive.ics.uci.edu/ml/datasets/APS+Failure+at+Scania+Trucks

> Due to dataset size restrictions, CSV files are not included in this repository.

---

## 🧠 Methodology

### Data Processing
- Missing value handling (median imputation)
- Numeric coercion
- Feature scaling using StandardScaler
- Removal of zero-variance features

### Model
- Logistic Regression
- Class weighting to handle imbalance
- Threshold = 0.5

### Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC
- Precision–Recall Curve
- APS Cost Function:



  ---

## 📈 Results

The model achieves strong recall while minimizing APS-specific cost.  
The system is suitable for predictive maintenance scenarios where false negatives are highly penalized.

---

## 🚀 Future Improvements

- Threshold tuning for minimum APS cost
- Random Forest / Gradient Boosting comparison
- Cross-validation
- Feature importance analysis
- Deep learning model comparison (LSTM)

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn

---

## 👨‍💻 Author

Kesava Bobbili  
B.Tech – Electronics and Communication Engineering  
IIITDM Kancheepuram

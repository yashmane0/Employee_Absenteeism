# 🚧 Employee Absenteeism Prediction using Machine Learning

> 🎯 “Predict absenteeism before it becomes a problem.”

This project predicts whether an employee is likely to have high absenteeism using historical workplace data. The goal is to support HR departments in early detection, resource planning, and productivity optimization.

---

## 📌 Problem Statement

Employee absenteeism affects productivity, scheduling, and operations in many organizations. The inability to forecast absenteeism leads to workflow disruptions and inefficient resource usage. This project builds a predictive model using classification algorithms to identify employees at high risk of absenteeism.

---

## 💡 Proposed Solution

- Analyze historical absenteeism data from Excel file (`Absent_at_work.xls`)
- Preprocess the data (remove ID, handle nulls, rename columns)
- Engineer features and encode categorical variables
- Train machine learning models to classify absenteeism as high or low
- Evaluate and compare models using appropriate metrics

---

## ⚙️ Technologies & Libraries Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn, hvPlot
- Scikit-learn
- XGBoost
- Pickle (for saving models)

---

## 🧪 System Workflow

1. **Data Preprocessing**
   - Drop unnecessary columns (e.g., ID)
   - Handle missing values
   - Replace spaces in column names
   - Encode categorical features (group reasons for absence into 4 groups)
   - Normalize numeric values using `MinMaxScaler` and `StandardScaler`

2. **Feature Engineering**
   - One-hot encoding for categorical variables
   - Education levels: 1 → 0 (basic), 2/3/4 → 1 (higher)
   - Target variable: 
     - `1` if absenteeism hours > median
     - `0` otherwise

3. **Model Training**
   - Algorithms: Logistic Regression, Random Forest, SVM, XGBoost
   - Train-test split: 70/30
   - Use pipelines for consistent preprocessing
   - Hyperparameter tuning with `GridSearchCV`
   - Model persistence with `pickle`

4. **Model Evaluation**
   - Accuracy, Confusion Matrix, Precision, Recall, F1-score, ROC-AUC
   - ROC and Precision-Recall curves

---

## ✅ Results

- **Best model**: XGBoost with ~76.84% accuracy
- **F1-score**: ~0.77 indicating good balance between precision and recall
- **Confusion matrix**:
  - TP = 149 (correct high absentee)
  - TN = 196 (correct low absentee)
  - FP = 54, FN = 50
- **ROC AUC**: >0.75 (strong classification capability)

---

## Images
![image](https://github.com/user-attachments/assets/bdf57497-0c91-4866-8ff7-781d09797290)
![image](https://github.com/user-attachments/assets/af22afb1-b6d9-4938-9f5a-ba3dd18c2ba5)
![image](https://github.com/user-attachments/assets/29ec16aa-f905-466f-a582-23f30697feb1)
![image](https://github.com/user-attachments/assets/faba3840-96c3-4fac-8d6a-d323b7379568)
![image](https://github.com/user-attachments/assets/04ef0959-c247-4a73-b6de-2c0fec675dce)
![image](https://github.com/user-attachments/assets/38c5af42-832b-4d6d-9512-6e70ebc7062d)

---

## 🔮 Future Scope

- Use real-time attendance or biometric data
- Integrate with HR systems or cloud-based dashboards
- Explore advanced ML (e.g., Neural Networks, AutoML, LSTM)
- Scale to large organizations with multiple branches

---


---

## 📚 References

- IEEE Paper: "Predicting Employee Absenteeism using Machine Learning" – 2020  
- IJCSIT: "Classification Algorithms for Predicting Absenteeism" – 2021  
- Kaggle Notebooks, GitHub Repos, Scikit-learn & XGBoost documentation

---

## 👤 Author

**Yash Mahendra Mane**  
Email: maneyash00@gmail.com   

---





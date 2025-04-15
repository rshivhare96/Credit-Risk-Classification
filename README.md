# Credit Risk Classification

This project focuses on predicting the success or rejection of loan applications using applicant data and credit-related features. The objective is to build a robust classification model for credit risk assessment, helping financial institutions make informed lending decisions.

---

## 📂 Data

The dataset includes loan applications along with associated credit features for each applicant. It comprises three files:

- **loan_applications.csv**: Contains loan application details and the target variable (`Success`).
- **credit_features_subset.csv**: Contains credit history information and account statistics.
- **loan_data_dictionary.csv**: Provides detailed explanations of each feature.

These datasets were merged and processed to create a comprehensive data foundation for modeling.

---

## 🔍 Analysis Workflow

The project is implemented in Python and includes the following steps:

- Data merging and cleaning  
- Handling missing values and negative placeholders  
- Outlier treatment using IQR-based capping and log transformation  
- Feature engineering (e.g., debt-to-income ratio, account activity features)  
- Date-based feature extraction from `ApplicationDate`  
- Exploratory Data Analysis (EDA)  
- Correlation heatmaps and feature selection  
- Model building using **Random Forest Classifier**  
- Evaluation using classification metrics  

---

## ⚙️ Models Used

The following machine learning model is implemented:

- ✅ **Random Forest Classifier** (Primary model)

Other techniques applied:

- Outlier handling  
- Log transformations for skewed data  
- Median imputation for missing values  
- Class balance handling (to be enhanced in future versions)  

---

## 📊 Key Findings

- Achieved **90% overall accuracy**, but faced **class imbalance**.
- **Precision for class 0**: 0.91 (non-success prediction is strong)  
- **Precision for class 1**: 0.38 (success prediction is weaker)  

This suggests the model is biased toward the majority class and can benefit from balancing techniques such as SMOTE or class-weight tuning.

---

## 🛠️ Libraries Used

- **Data Manipulation**: `pandas`, `numpy`  
- **Visualization**: `matplotlib`, `seaborn`  
- **Machine Learning**: `scikit-learn`  
- **Feature Engineering**: `LabelEncoder`, `SelectKBest`, `RobustScaler`  

---

## 📁 Notebooks & Scripts

- `credit_risk_model.ipynb`: Contains full workflow including EDA, preprocessing, feature engineering, model building, and evaluation.

---

## ✅ Usage

To reproduce the analysis:

1. Clone the repository  
2. Place the dataset CSV files in the project directory  
3. Run `credit_risk_model.ipynb` end-to-end  
4. Evaluate results using classification metrics (precision, recall, F1-score)  

**Optional Improvements**:
- Handle class imbalance via SMOTE or class weighting  
- Experiment with other models like XGBoost or Logistic Regression  
- Perform hyperparameter tuning for Random Forest  

---

## 👤 Author

**Rohit Shivhare**  
[LinkedIn](https://www.linkedin.com/in/rohit-shivhare-a857a4233/)  
*MSc Data Science – Brunel University, London*

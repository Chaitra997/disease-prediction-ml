# Disease Prediction using Machine Learning

This project aims to build a predictive machine learning model that can determine whether a patient is likely to have a disease based on clinical features.

## 🧠 What I Did

- Analyzed and preprocessed patient data (training: 4000 samples, testing: 1000 samples).
- Ensured **data integrity** by checking for and confirming no missing values.
- Addressed **class imbalance** using **Borderline-SMOTE**, boosting performance on minority class predictions.
- Applied **feature standardization** to improve model convergence.
- Used **RandomForestClassifier** with **GridSearchCV** for hyperparameter tuning.
- Implemented **Stratified 5-Fold Cross Validation** to ensure robust performance.
- Evaluated model using **ROC-AUC**, **accuracy**, **precision**, **recall**, and **F1 score**.
- Made predictions on unseen test data and saved results to a CSV file.

## 📊 Dataset Details

- `Disease_train.csv`: 4000 records, includes `patient_id`, 10 numerical features, and `diagnosis` (target).
- `Disease_test.csv`: 1000 records, includes `patient_id` and 10 numerical features.

## ✅ Results

| Metric       | Validation Set | Cross-Validation |
|--------------|----------------|------------------|
| ROC-AUC      | 0.9776         | 0.9482           |
| Accuracy     | 0.9777         | 0.9482           |
| Precision    | 0.9813         | 0.9287           |
| Recall       | 0.9735         | 0.9713           |
| F1 Score     | 0.9774         | 0.9495           |

## 🛠️ Technologies Used

- Python (Pandas, NumPy, Scikit-learn)
- SMOTE (Imbalanced-learn)
- GridSearchCV
- Stratified K-Fold Cross Validation
- Matplotlib & Seaborn for visualization

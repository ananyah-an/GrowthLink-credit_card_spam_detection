💳 Credit Card Fraud Detection using XGBoost & SHAP

📌 Project Summary

This project identifies fraudulent credit card transactions using machine learning. It combines XGBoost for prediction, SMOTE to handle class imbalance, and SHAP for model explainability.

📦 Libraries Used

pandas, numpy

scikit-learn, imbalanced-learn

xgboost

seaborn, matplotlib

shap

📁 Dataset

Source: Kaggle - Fraud Detection

File Used: fraudTrain.csv

⚙️ Steps to Run

Install required packages:

pip install pandas numpy scikit-learn imbalanced-learn xgboost shap seaborn matplotlib

Place fraudTrain.csv in your working directory.

Run the script in your IDE / Jupyter Notebook / Google Colab.

🔍 Feature Engineering

Extracted datetime features: hour, day, month, year

Derived features: age, amt_per_pop, merchant_distance

Label encoded: merchant, category, gender, job, city, state

🧐 Model

Model: XGBoostClassifier

Handling Imbalance: SMOTE

Scaling: StandardScaler

📊 Results

Classification Report:

Class 0 (Legit) → Precision: 1.00 | Recall: 0.99 | F1: 0.99  
Class 1 (Fraud) → Precision: 0.32 | Recall: 0.95 | F1: 0.48  

Accuracy: 0.99
ROC AUC Score: 0.9698

👌 High fraud recall — most fraudulent transactions are correctly detected.

🔎 Model Explainability with SHAP

Waterfall Plot: individual prediction explanation

Beeswarm Plot: global feature importance

Summary Plot: top contributing features

✅ Conclusion

Effective fraud detection with a balance of precision and recall

Interpretability via SHAP builds trust in model decisions

Ready to be integrated into real-time applications or exposed via API

Made with ❤️ using Python & Machine Learning


💳 CardDefender

CardDefender is an interactive AI-powered web application that detects fraudulent credit card transactions using anomaly detection techniques. Built using Streamlit and scikit-learn, it allows users to upload their own datasets and receive instant insights into suspicious transactions and can be downloaded as csv file.

🚀 Features

- 🕵️‍♂️ Fraud Detection using Isolation Forest
- 📂 Upload Your Dataset via Streamlit interface
- 📊 Interactive Visualizations for fraud/legit transactions
- 🧾 Downloadable Results as a clean CSV file
- ⚙️ Automatic Preprocessing (scaling, cleaning)
- 🎯 Powered by Unsupervised Machine Learning

🧠 Anomaly Detection Models (Training Script)

The backend also includes a script that compares:
- Isolation Forest  
- Local Outlier Factor  
- One-Class SVM

These models are tested using the [Kaggle Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

📦 Getting Started

✅ Requirements

- Python 3.x  
- Streamlit  
- scikit-learn  
- pandas  
- seaborn  
- matplotlib  

📁 Dataset Format
The app expects a CSV with the following structure:

Numerical features: V1, V2, ..., V28, Amount

A Time column (optional — will be dropped automatically)

A Class column with:

0 = Legit

1 = Fraud

📊 Output Visualizations
Summary of uploaded data

Number of fraudulent vs. legitimate transactions

Downloadable CSV of predicted frauds

Highlighted fraud cases directly in the UI

📉 Example Results (Training Script)
In fraud_model_test.py, three models are evaluated:

Isolation Forest

Local Outlier Factor

One-Class SVM

Each prints:

Confusion matrix

Classification report (precision, recall, F1-score)

This helps evaluate which model performs best for unsupervised fraud detection tasks.

🔒 Disclaimer
This tool is built for educational and research purposes only.
Do not use this model for real-world financial decision-making without proper validation.

📜 License
This project is licensed under the MIT License.



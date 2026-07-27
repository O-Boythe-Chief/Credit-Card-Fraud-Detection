# 💳 Credit Card Fraud Detection
### Machine Learning-Based Fraud Detection using Logistic Regression & Random Forest

A machine learning project that detects fraudulent credit card transactions by analyzing transaction patterns and customer behavior. The project compares **Logistic Regression** and **Random Forest** classifiers to identify the most effective model for binary fraud detection.

---

# 📌 Project Overview

Credit card fraud has become one of the most significant challenges in the financial industry. Detecting fraudulent transactions quickly and accurately helps financial institutions minimize financial losses while protecting customers.

This project implements a complete fraud detection pipeline, including:

- Data preprocessing
- Class imbalance analysis
- Feature scaling
- Model training
- Model evaluation
- Fraud probability prediction
- Model serialization

---

# 🎯 Objectives

- Detect fraudulent credit card transactions.
- Compare Logistic Regression and Random Forest classifiers.
- Evaluate model performance using multiple classification metrics.
- Predict fraud probability for unseen transactions.
- Save the trained model for future deployment.

---

# 🏗️ Project Workflow

```text
             Credit Card Transaction Dataset
                          │
                          ▼
                 Data Preprocessing
                          │
        ┌─────────────────┴─────────────────┐
        │                                   │
   Data Cleaning                    Feature Scaling
        │                                   │
        └─────────────────┬─────────────────┘
                          │
                   Train-Test Split
                          │
        ┌─────────────────┴─────────────────┐
        │                                   │
 Logistic Regression            Random Forest
        │                                   │
        └─────────────────┬─────────────────┘
                          │
                 Model Evaluation
                          │
                          ▼
             Fraud Probability Prediction
```

---

# ✨ Features

- Credit card fraud classification
- Transaction data preprocessing
- Feature scaling using StandardScaler
- Logistic Regression implementation
- Random Forest implementation
- Fraud probability prediction
- Class distribution visualization
- Confusion Matrix
- Classification Report
- ROC-AUC evaluation
- Model export using Joblib

---

# 🧠 Machine Learning Models

## 📈 Logistic Regression

A linear classification algorithm used as a baseline model for binary fraud detection.

### Advantages

- Fast training
- Easy interpretation
- Efficient for large datasets
- Low computational cost

---

## 🌳 Random Forest Classifier

An ensemble learning algorithm that combines multiple decision trees to improve prediction accuracy and robustness.

### Advantages

- Handles complex non-linear patterns
- High prediction accuracy
- Robust against overfitting
- Performs well on tabular financial data

---

# 📊 Dataset

The project uses a credit card transaction dataset containing anonymized transaction features along with a target label indicating whether a transaction is fraudulent.

The target variable is:

```text
Class

0 → Legitimate Transaction
1 → Fraudulent Transaction
```

> **Note:** Due to GitHub file size limitations, the dataset is not included in this repository. Please download it separately and place it in the project directory before running the notebook.

---

# ⚙️ Data Preprocessing

The notebook performs the following preprocessing steps:

- Load transaction dataset
- Inspect dataset dimensions
- Analyze fraud class distribution
- Feature scaling using StandardScaler
- Separate features and target labels
- Split into training and testing datasets

---

# 📈 Exploratory Data Analysis

The project visualizes the dataset to better understand fraud distribution before training.

Visualizations include:

- Dataset shape
- Fraud vs Legitimate transaction distribution
- Class imbalance analysis

---

# 🧪 Model Training

The dataset is divided into:

- Training Set (80%)
- Testing Set (20%)

using Scikit-learn's `train_test_split()` function.

Both models are trained using identical datasets for fair comparison.

---

# 📈 Evaluation Metrics

The models are evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC Score
- Fraud Probability

These metrics provide a comprehensive evaluation of classification performance on an imbalanced dataset.

---

# 📊 Visualizations

The notebook includes several visual analyses, including:

- Class Distribution Plot
- Confusion Matrix
- Classification Report
- ROC-AUC Performance
- Fraud Probability Prediction

Additional visualizations that can be added in future versions include:

- ROC Curve
- Precision-Recall Curve
- Feature Importance
- SHAP Explainability

---

# 💾 Model Saving

The trained Random Forest model is saved using **Joblib** for deployment and future inference.

```python
import joblib

joblib.dump(rf_model, "fraud_model.pkl")
```

The saved model can later be integrated into a web application or REST API.

---

# 🛠️ Technologies Used

| Category | Technology |
|----------|------------|
| Language | Python |
| Machine Learning | Scikit-learn |
| Data Processing | NumPy, Pandas |
| Visualization | Matplotlib, Seaborn |
| Model Serialization | Joblib |
| Notebook | Jupyter Notebook |

---

# 📂 Project Structure

```text
Credit-Card-Fraud-Detection/
│
├── Credit Card Fraud Detection Model.ipynb
├── fraud_model.pkl
├── README.md
├── requirements.txt
└── LICENSE
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Credit-Card-Fraud-Detection.git
```

Navigate to the project directory

```bash
cd Credit-Card-Fraud-Detection
```

Install the required dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Project

Launch Jupyter Notebook

```bash
jupyter notebook "Credit Card Fraud Detection Model.ipynb"
```

Run all notebook cells sequentially to:

1. Load the dataset
2. Preprocess the data
3. Train both models
4. Evaluate performance
5. Predict fraud probability
6. Save the trained model

---

# 📦 Required Libraries

```text
numpy
pandas
matplotlib
seaborn
scikit-learn
joblib
```

Install manually

```bash
pip install numpy pandas matplotlib seaborn scikit-learn joblib
```

or

```bash
pip install -r requirements.txt
```

---

# 📊 Results

The project compares:

- Logistic Regression
- Random Forest

using identical training and testing datasets.

Model performance is evaluated using multiple classification metrics to determine the most effective fraud detection algorithm.

The trained Random Forest model is saved for future deployment.

---

# 🔮 Future Improvements

- Handle class imbalance using SMOTE
- Hyperparameter optimization with GridSearchCV or Optuna
- XGBoost and LightGBM implementation
- SHAP explainability
- Feature importance visualization
- ROC and Precision-Recall curves
- Real-time fraud detection API
- Web application using Flask or FastAPI

---

# 🤝 Contributing

Contributions are welcome!

Possible improvements include:

- Better preprocessing techniques
- Additional classification algorithms
- Enhanced visualizations
- Model optimization
- Deployment support

Feel free to open an Issue or submit a Pull Request.

---

# 📜 License

This project is licensed under the MIT License.

---

# 👨‍💻 Author

**Arnab Mohanta**

If you found this project useful, consider giving it a ⭐ on GitHub!

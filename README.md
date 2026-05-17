# 📧 Email Spam Detection

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Machine Learning](https://img.shields.io/badge/ML-Classification-green.svg)
![Accuracy](https://img.shields.io/badge/Accuracy-98%25-brightgreen.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-NLP%20%7C%20ML-orange.svg)

---

## 📌 Project Overview
This project builds a **machine learning-based spam email detection system** using Natural Language Processing (NLP) techniques.  
It classifies emails into:

- 📩 **Ham (Legitimate emails)**
- 🚫 **Spam (Unwanted / malicious emails)**

Spam detection improves cybersecurity by preventing phishing attacks, scams, and unwanted advertisements.


---

## 🗂️ Project Structure


Email-Spam-Detection/
│
├── data/
│ └── emails.csv
│
├── notebooks/
│ ├── EDA.ipynb
│ ├── preprocessing.ipynb
│ └── modeling.ipynb
│
├── models/
│ ├── svm_model.pkl
│ ├── rf_model.pkl
│
├── src/
│ ├── preprocessing.py
│ ├── feature_engineering.py
│ ├── train.py
│ └── predict.py
│
├── visuals/
│ ├── plots/
│ └── wordcloud.png
│
├── requirements.txt
└── README.md


---

⚙️ Workflow
1️⃣ Data Loading
import pandas as pd

df = pd.read_csv("emails.csv")
2️⃣ Data Preprocessing

This step includes:

Handling missing values
Label encoding (spam = 1, ham = 0)
Tokenization using NLTK
Stopwords removal
Stemming using Porter Stemmer
from nltk.stem import PorterStemmer

stemmer = PorterStemmer()
3️⃣ Feature Engineering
Extract email length features
Apply TF-IDF vectorization
from sklearn.feature_extraction.text import TfidfVectorizer

vectorizer = TfidfVectorizer()
X = vectorizer.fit_transform(df['text'])
4️⃣ Feature Selection
Chi-Square Test → for relationship between categorical variables
Mutual Information → for feature importance
5️⃣ Model Training

Models used:

Multinomial Naive Bayes
Logistic Regression
Decision Tree
Support Vector Machine (SVM)
Random Forest
K-Nearest Neighbors (KNN)

Example (SVM model):

from sklearn.svm import SVC

model = SVC(kernel='linear')
model.fit(X_train, y_train)
6️⃣ Model Evaluation

Evaluation metrics:

Accuracy
Precision
Recall
F1-score

🏆 Best Model Accuracy: 98%

📊 Data Visualization
📈 Count Plot → Spam vs Ham distribution
🥧 Pie Chart → Class distribution
📊 Bar Plot → Email statistics
☁️ WordCloud → Frequent spam words
📉 KDE Plot → Email length distribution
🔥 Correlation Heatmap → Feature relationships
🤖 Machine Learning Models Comparison
Model	Description
Naive Bayes	Best for text classification
Logistic Regression	Linear probabilistic model
Decision Tree	Rule-based learning
SVM	Margin-based classifier
Random Forest	Ensemble of decision trees
KNN	Distance-based classifier
📈 Results
🎯 Accuracy: 98%
📌 High Precision & Recall
📌 Strong F1-score
📌 Robust spam detection system
🚀 Conclusion

This project demonstrates the power of Machine Learning + NLP in detecting spam emails effectively. It significantly improves email security and reduces phishing risks.

🔮 Future Work
Implement deep learning models (LSTM, BERT)
Improve feature selection techniques
Handle imbalanced datasets
Deploy as real-time web application (Flask / Streamlit)
🔐 Impact
Enhances email security
Prevents phishing and scams
Improves user experience
Reduces inbox clutter
📦 Installation
pip install -r requirements.txt
▶️ Run Project
python src/train.py
python src/predict.py
⭐ Acknowledgements

Thanks to all contributors and instructors supporting this project.ntReference[oaicite:9]{index=9}

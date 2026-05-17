# Email Spam Detection

<div align="center">

# 📧 Email Spam Detection using Machine Learning

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Scikit--Learn-orange)
![NLP](https://img.shields.io/badge/NLP-NLTK-green)
![Accuracy](https://img.shields.io/badge/Accuracy-98%25-brightgreen)
![Status](https://img.shields.io/badge/Status-Completed-success)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

A Machine Learning and NLP-based project for detecting spam emails with high accuracy using multiple classification algorithms.

</div>

---

# 📌 Table of Contents

- [Introduction](#-introduction)
- [Project Features](#-project-features)
- [Technologies Used](#-technologies-used)
- [Data Preprocessing](#-data-preprocessing)
- [Data Visualization](#-data-visualization)
- [Feature Selection & Extraction](#-feature-selection--extraction)
- [Machine Learning Models](#-machine-learning-models)
- [Results](#-results)
- [Project Workflow](#-project-workflow)
- [Installation](#-installation)
- [Usage](#-usage)
- [Future Improvements](#-future-improvements)
- [Conclusion](#-conclusion)
- [Author](#-author)
- [License](#-license)

---

# 📖 Introduction

Spam email detection is an important application of **Machine Learning** and **Natural Language Processing (NLP)**.

Spam emails may include:
- Advertisements
- Fraudulent messages
- Malware links
- Phishing attacks

This project builds a machine learning system capable of automatically classifying emails into:

- ✅ **Ham (Legitimate Email)**
- ❌ **Spam Email**

The project combines:
- Data preprocessing
- NLP techniques
- Feature engineering
- Data visualization
- Multiple machine learning models

---

# 🚀 Project Features

✅ Email text preprocessing  
✅ Tokenization and stemming  
✅ TF-IDF feature extraction  
✅ Multiple ML classification models  
✅ Exploratory Data Analysis (EDA)  
✅ Data visualization using Seaborn & Plotly  
✅ Spam word cloud generation  
✅ High classification accuracy (~98%)  
✅ Feature selection using Chi-Square & Mutual Information  

---

# 🛠 Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming Language |
| NumPy | Numerical Computing |
| Pandas | Data Manipulation |
| Matplotlib | Data Visualization |
| Seaborn | Statistical Visualization |
| Plotly Express | Interactive Charts |
| NLTK | Natural Language Processing |
| Scikit-learn | Machine Learning |

---

# 🔄 Data Preprocessing

## ✅ Handling Null Values
- The dataset was checked for missing values.
- No null values were found.

---

## ✅ Outlier Detection
Outliers were analyzed using:
- Box plots
- Statistical methods

The engineered feature:

```python
length_times_emails
```

contained 527 outliers which were handled using Min-Max replacement.

---

## ✅ Encoding Categorical Variables

The labels were converted into numerical values:

| Label | Encoded Value |
|---|---|
| Ham | 0 |
| Spam | 1 |

---

## ✅ Tokenization

Text was split into tokens (words).

Example:

```python
"Free money now!"
→ ["Free", "money", "now"]
```

---

## ✅ Stemming

Used **Porter Stemmer** from NLTK to reduce words to root form.

Example:

```python
playing → play
played → play
plays → play
```

---

## ✅ Feature Engineering

Additional features extracted:
- Email subject length
- Number of sent emails
- Email text length

---

# 📊 Data Visualization

The project includes multiple visualization techniques:

| Visualization | Purpose |
|---|---|
| Count Plot | Label distribution |
| Pie Chart | Spam vs Ham percentage |
| Bar Plot | Sent emails comparison |
| Scatter Plot | Relationship analysis |
| Box Plot | Outlier detection |
| Word Cloud | Common spam words |
| KDE Plot | Density distribution |
| Histogram | Email length distribution |
| Correlation Heatmap | Feature relationships |

---

# 🔍 Feature Selection & Extraction

## 📌 Chi-Square Test

Used to determine the relationship between:
- Email labels
- Email content

Implemented using:

```python
chi2_contingency()
```

---

## 📌 TF-IDF Vectorization

Used:

```python
TfidfVectorizer
```

to convert text into numerical vectors.

### Benefits:
- Highlights important words
- Reduces effect of common words
- Improves model performance

---

## 📌 Mutual Information

Used to measure feature importance and relevance in predicting spam emails.

---

# 🤖 Machine Learning Models

## 1️⃣ Multinomial Naive Bayes
- Fast and efficient
- Ideal for text classification
- Handles high-dimensional data

---

## 2️⃣ Logistic Regression
- Binary classification algorithm
- Simple and effective

---

## 3️⃣ Decision Tree
Tree-based classification model.

### Entropy Formula

```math
H(p) = -p log₂(p) - (1-p) log₂(1-p)
```

---

## 4️⃣ Support Vector Machine (SVM)
- Finds optimal separating hyperplane
- Supports linear and non-linear classification

---

## 5️⃣ Random Forest
- Ensemble learning algorithm
- Reduces overfitting
- High accuracy performance

---

## 6️⃣ K-Nearest Neighbors (KNN)
- Distance-based classifier
- Classifies using nearest neighbors

---

# 📈 Results

## ✅ Model Performance

The project achieved approximately:

# 🎯 Accuracy: **98%**

### Evaluation Metrics:
- Accuracy
- Precision
- Recall
- F1-Score

The classifier demonstrated strong capability in distinguishing spam emails from legitimate emails.

---

# 🔁 Project Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
Text Preprocessing
   ↓
Tokenization & Stemming
   ↓
Feature Extraction (TF-IDF)
   ↓
Feature Selection
   ↓
Train/Test Split
   ↓
Model Training
   ↓
Prediction
   ↓
Evaluation
```

---

# ⚙️ Installation

## Clone the repository

```bash
git clone https://github.com/your-username/email-spam-detection.git
```

## Navigate to project folder

```bash
cd email-spam-detection
```

## Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Usage

Run the notebook or Python script:

```bash
python spam_detection.py
```

or open:

```bash
Email_Spam_Detection.ipynb
```

using Jupyter Notebook.

---

# 📌 Future Improvements

🚀 Real-time spam detection  
🚀 Deep Learning models (LSTM/BERT)  
🚀 Web application deployment  
🚀 Better handling of imbalanced datasets  
🚀 API integration  

---

# 🏁 Conclusion

This project demonstrates the effectiveness of combining:
- Machine Learning
- Natural Language Processing
- Feature Engineering

to build a highly accurate spam email classifier.

The system successfully detects spam emails and improves email security and user experience.

---

# 👨‍💻 Author

## Ahdab Osama

Machine Learning & AI Enthusiast

---

# 📄 License

This project is licensed under the MIT License.

# 📧 Spam Email Detection System using Machine Learning

## 📌 Project Overview

This project detects whether a message is **Spam** or **Ham (Legitimate)** using Machine Learning and Natural Language Processing (NLP).

The project compares three machine learning algorithms:

- Logistic Regression
- Multinomial Naive Bayes
- Linear Support Vector Machine (SVM)

The text messages are converted into numerical features using **TF-IDF (Term Frequency–Inverse Document Frequency)** before model training.

## 🎯 Objective

The main objective of this project is to build a machine learning system that can automatically classify email/message text as:

- 🚫 **Spam**
- ✅ **Ham (Legitimate)**

## 📂 Dataset

The project uses a dataset containing **5,572 messages** with two columns:

- `Category` — spam or ham
- `Message` — the message text

The notebook converts the labels into numerical form:

- `spam = 0`
- `ham = 1`

Place the dataset in the project root with this filename:

```text
mail_data.csv
```

## 🔄 Project Workflow

```text
Dataset
   ↓
Data Cleaning & Pre-processing
   ↓
Exploratory Data Analysis (EDA)
   ↓
Train-Test Split
   ↓
TF-IDF Vectorization
   ↓
Model Training
   ↓
Model Evaluation
   ↓
Best Model Selection
   ↓
Spam/Ham Prediction
```

## 🧠 Machine Learning Models

### 1. Logistic Regression
A classification algorithm used to predict whether a message belongs to the spam or ham class.

### 2. Multinomial Naive Bayes
A probabilistic classification algorithm that works particularly well with text and word-frequency-based features.

### 3. Linear SVM
A Support Vector Machine classifier that finds a decision boundary to separate spam and legitimate messages.

## 🔤 Feature Extraction — TF-IDF

TF-IDF converts text into numerical values that machine learning models can process.

It gives higher importance to words that are useful for distinguishing between messages while reducing the importance of very common words.

## 📊 Model Performance

According to the project notebook:

| Model | Accuracy | Precision | Recall | F1 Score |
|---|---:|---:|---:|---:|
| Logistic Regression | 96.68% | 96.29% | 100.00% | 98.11% |
| Multinomial Naive Bayes | 97.31% | 96.97% | 100.00% | 98.46% |
| Linear SVM | **98.21%** | **98.06%** | **99.90%** | **98.97%** |

🏆 **Best Model: Linear SVM**

The notebook selects Linear SVM based on the highest F1 score.

## 🧪 Example Predictions

The project tests messages such as:

- Promotional/prize messages → 🚫 Spam
- Normal meeting messages → ✅ Ham
- Urgent account-verification messages → 🚫 Spam

## 🛠️ Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- WordCloud
- Scikit-learn
- Jupyter Notebook
- NLP
- TF-IDF
- Logistic Regression
- Naive Bayes
- Linear SVM

## 📁 Project Structure

```text
spam-email-detection-ml/
│
├── spam_email_detection.ipynb
├── mail_data.csv
├── README.md
├── requirements.txt
└── .gitignore
```

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/spam-email-detection-ml.git
cd spam-email-detection-ml
```

### 2. Install the required libraries

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook
```

Open:

```text
spam_email_detection.ipynb
```

Make sure `mail_data.csv` is present in the same folder before running the notebook.

## 👩‍💻 Project By

**Anshi Sharma**

B.Tech — CSE-AIML  
Jaipur National University

## ⭐ Project Highlights

- Text classification using Machine Learning
- NLP-based feature extraction
- TF-IDF vectorization
- Comparison of three classification algorithms
- Evaluation using Accuracy, Precision, Recall and F1 Score
- Best model selection using F1 Score
- Final spam/ham prediction system

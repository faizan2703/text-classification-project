# 📘 **IMDB Movie Reviews – Text Classification**

This project builds an end-to-end **sentiment-analysis** pipeline using the **IMDB Movie Reviews Dataset**.
It includes text preprocessing, feature extraction using BoW and TF-IDF, and machine-learning models such as **Random Forest**, **Gaussian Naive Bayes**, and **Multinomial Naive Bayes**.

---

## 🚀 **Project Overview**

The goal is to classify movie reviews as **positive** or **negative** using classic NLP and ML techniques.
The best model achieved **~85% test accuracy**.

---

## 📂 **Project Workflow**

### **1. Data Preprocessing**

* Lowercasing text
* Removing punctuation
* Removing stopwords
* Tokenization
* Cleaning unwanted symbols
* Preparing clean text for vectorization

---

### **2. Feature Engineering**

Used two main vectorization methods:

1️⃣ **Bag-of-Words (BoW)**
2️⃣ **TF-IDF Vectorizer**

Both were tested with different n-gram settings (unigram, bigram).

---

### **3. Models Used**

| Model                        | Description                       | Result                        |
| ---------------------------- | --------------------------------- | ----------------------------- |
| **Random Forest Classifier** | Ensemble decision-tree classifier | ⭐ ~85% accuracy               |
| **Multinomial Naive Bayes**  | Best for sparse TF-IDF/BoW data   | ⭐ Good performance            |
| **Gaussian Naive Bayes**     | Applied for comparison            | Lower accuracy on sparse text |

The **best results** came from **TF-IDF + MultinomialNB / RandomForest**.

---

## 📊 **Results**

* **Best Accuracy:** **~85%**
* **Best Features:** TF-IDF (ngram_range up to bigrams)
* **Best Classifier:** Random Forest / MultinomialNB

---

## 🛠️ **Tech Stack**

* **Python**
* **scikit-learn**
* **NLTK / re / string**
* **pandas, NumPy**
* **matplotlib / seaborn** (optional for plots)

---

## 📁 **How to Run**

### Install required libraries:

```bash
pip install -r requirements.txt
```

### Run notebook or script:

```bash
python main.py
```

or open the `.ipynb` file.

---

## 📝 **Key Learnings**

* NLP preprocessing techniques
* Difference between BoW and TF-IDF
* How ML models behave with sparse vectors
* Importance of n-grams & feature size
* Comparing Naive Bayes vs Random Forest for text

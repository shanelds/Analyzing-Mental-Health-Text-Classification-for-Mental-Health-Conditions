# Mental Health Text Classification

This project aims to classify a person’s mental or emotional state based on short text statements (such as social media posts or messages). The goal is to support in early detection of mental health conditions through natural language processing (NLP).

---

## 🎯 Goal
The goal of this project is to explore whether machine learning models can accurately classify emotional and mental health states from short texts. We compare several models and aim to identify the most effective one for predicting mental health conditions.

---

## 📊 Visual Abstract

The figure below illustrates the overall workflow of our project — from input text to model processing and final prediction:

![Visual Abstract](https://github.com/shanelds/Analyzing-Mental-Health-Text-Classification-for-Mental-Health-Conditions/blob/main/VISUAL%20ABSTRACT.png?raw=true)

---

## 📂 Datasets

The project uses a combined dataset containing over 53,000 labeled text statements related to mental health states. The main sources include:

* Kaggle - Mental Health Text Dataset
  
[https://www.kaggle.com/datasets/tannergrossmann/mental-health-text](https://www.kaggle.com/datasets/suchintikasarkar/sentiment-analysis-for-mental-health)

* Additional dataset
  
[https://www.kaggle.com/datasets/praveengovi/emotions-dataset-for-nlp](https://github.com/rafalposwiata/depression-detection-lt-edi-2022)

-All datasets were merged and cleaned for training and evaluation.


---

## 🤖 Models
We applied and compared several machine learning models to classify mental health conditions from text:

- Naive Bayes
- Logistic Regression (TF-IDF)
- Logistic Regression (n-grams)
- SVM (n-grams)
- Random Forest
- XGBoost
- BERT
- Distil-BERT — Best performance with an accuracy of 79.3%

---

## 📝 Evaluation
We evaluated the model performance using the following classification metrics:

Precision

Accuracy

Recall

F1 Score

These metrics helped to assess how well each model handled different mental health categories and supported the selection of the best model (Distil-BERT).

We also used a confusion matrix to visualize the distribution of predictions across categories and identify potential misclassifications.

---

## 📊 Results Summary

| Model                         | Accuracy  | Precision | Recall    | F1-Score  |
| ----------------------------- | --------- | --------- | --------- | --------- |
| Naive Bayes                   | 70.0%     | 71.0%     | 69.0%     | 70.0%     |
| Logistic Regression (TF-IDF)  | 74.0%     | 74.0%     | 74.0%     | 73.0%     |
| Logistic Regression (n-grams) | 75.0%     | 74.0%     | 74.0%     | 74.0%     |
| SVM (n-grams)                 | 73.0%     | 73.0%     | 73.0%     | 73.0%     |
| Random Forest                 | 69.0%     | 72.0%     | 68.0%     | 66.0%     |
| XGBoost                       | 75.0%     | 75.0%     | 75.0%     | 75.0%     |
| **Distil-BERT**               | **79.3%** | **76.7%** | **78.5%** | **78.0%** |

>  DistilBERT provided the highest classification accuracy (79.3%), making it the top-performing model for detecting mental health states from text.

---

## 🗂️ Folder Structure

├── data

│ ├── cleaned_data_readyy.csv

│ ├── cleaned_merged_dataset.zip

│ ├── final_data_.csv

│ └── merged_dataset.zip


├── notebook

│ └── FINAL_CODE.ipynb


├── presentation

│ ├── FINAL PROJECT - Analyzing Mental Health - text classification for mental health conditions.pdf

│ └── Interim Report – NLP Final Project_Analyzing Mental Health.pdf



├── README.md
└── VISUAL ABSTRACT.png

---


```markdown
## Quick Start

### Clone the repository
```bash
git clone https://github.com/shanelds/Analyzing-Mental-Health-Text-Classification-for-Mental-Health-Conditions.git
cd Analyzing-Mental-Health-Text-Classification-for-Mental-Health-Conditions
```

```bash
### Install dependencies
pip install -r requirements.txt
```

```bash
### Run the notebooks
jupyter notebook notebook/FINAL_CODE.ipynb
```
---

## Team

* Shahar Sadon
* Shanel Asulin
* Dudi Saadia

---



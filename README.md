# 🧠 NLP Final Project – Mental Health Text Classification

## 👥 Authors
Shahar Saadon | Dudi Saadia | Shanel Asulin  
Course Lecturer: Dr. Alexander (Sasha) Apartsin  

---

## 🎯 Project Overview
The project aims to classify a person’s mental or emotional state based on a short text message (e.g., post, chat).  
The classification helps detect mental health issues early and supports professionals in understanding emotional states.

⚠️ **Challenges**:
- Short and vague texts  
- Informal or casual language  
- Overlapping emotional categories  

---

## 📂 Data
- **Main dataset**: >53,000 labeled short text statements (7 mental health states)  
  Source: [Kaggle dataset](https://www.kaggle.com/datasets/suchintikasarkar/sentiment-analysis-for-mental-health)  
- **Additional dataset**: ~4,000 labeled statements (depression levels)  
  Source: [GitHub depression dataset](https://github.com/rafalposwiata/depression-detection-lt-edi-2022)  
- **Final dataset**: merged and cleaned CSV files (`final_data_.csv`, `cleaned_data_readyy.csv`)

---

## ⚙ Methods
- **Text preprocessing**: cleaning, TF-IDF (with/without n-grams), tokenization (WordPiece for BERT)
- **Models**:
  - 🟣 Naive Bayes  
  - 🟣 Logistic Regression (TF-IDF)  
  - 🟣 Logistic Regression (n-grams)  
  - 🟣 SVM (n-grams)  
  - 🟣 Random Forest  
  - 🟣 XGBoost  
  - 🟣 DistilBERT (frozen base / partial unfreeze / full fine-tuning)
- **Training**:
  - 80/20 train-test split (stratified)
  - DistilBERT: 4 epochs, small batch, gradient accumulation
- **Metrics**:
  - Accuracy
  - Macro & Weighted Precision / Recall / F1 (Macro-F1 prioritized)

---

## 📊 Key Results
| Model                      | Accuracy | Macro-F1 |
|----------------------------|----------|----------|
| Naive Bayes                | 70%      | 0.70     |
| Logistic Regression (TF-IDF)| 74%      | 0.73     |
| Logistic Regression (n-grams)| 75%     | 0.74     |
| SVM (n-grams)              | 73%      | 0.73     |
| Random Forest              | 69%      | 0.66     |
| XGBoost                    | 75%      | 0.75     |
| **DistilBERT (full FT)**    | **79.3%**| **0.79** |

---

## 📁 Repo Structure

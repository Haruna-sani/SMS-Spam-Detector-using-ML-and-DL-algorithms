# SMS-Spam-Detector-using-ML-and-DL-algorithms
# 📌 SMS Spam Classification: Comparative Analysis of ML & DL Models

## 📖 Project Overview
This project focuses on **classifying SMS messages as spam or ham (not spam)** using **Machine Learning (ML) and Deep Learning (DL) techniques**. The classification was performed using two feature extraction techniques:

1. **Bag of Words (BoW)**
2. **Term Frequency-Inverse Document Frequency (TF-IDF)**

The performance of three ML classifiers—**Random Forest (RF), XGBoost (XGB), and LightGBM (LGBM)**—was compared under both techniques. Additionally, **Deep Learning (DL) models (LSTM & Bi-LSTM)** were employed to analyze their effectiveness.

---
## 📊 Model Performance Comparison

### **1️⃣ Machine Learning Classifiers**
#### 🔹 Performance using **Bag of Words (BoW)**
| Model            | Accuracy  |
|-----------------|-----------|
| Random Forest (RF) | **0.9000** |
| XGBoost (XGB)   | **0.9800** |
| LightGBM (LGBM) | **0.8300** |

#### 🔹 Performance using **TF-IDF**
| Model            | Accuracy  |
|-----------------|-----------|
| Random Forest (RF) | **0.9830** |
| XGBoost (XGB)   | **0.9830** |
| LightGBM (LGBM) | **0.9839** |

### **2️⃣ Deep Learning Models**
| Model            | Accuracy  |
|-----------------|-----------|
| LSTM            | **0.8556** |
| Bi-LSTM         | **0.9839** |

---
## 🔎 **Observations & Insights**
1. **Bag of Words vs. TF-IDF:**
   - TF-IDF significantly **improved accuracy** for all ML classifiers compared to BoW.
   - LightGBM, which had **lower accuracy (0.83) in BoW**, improved drastically to **0.9839** with TF-IDF.

2. **XGBoost Performance:**
   - XGBoost performed exceptionally well in both **BoW (0.98)** and **TF-IDF (0.9830)**.
   - Its performance is comparable to deep learning models when using **TF-IDF**.

3. **Deep Learning vs. Machine Learning:**
   - LSTM's performance (**0.8556**) was **lower than ML models with TF-IDF**, suggesting that traditional ML models with proper feature extraction can be competitive.
   - Bi-LSTM achieved **0.9839**, making it the **best performing** model, tying with LightGBM under TF-IDF.

---
## 🚀 Conclusion
- **TF-IDF significantly enhanced performance** for all models.
- **XGBoost & Bi-LSTM performed the best**, making them ideal choices for SMS spam detection.
- **Traditional ML models (RF, XGB, LGBM) are still competitive** and, with proper feature engineering, can rival deep learning models.

---
## 🏗️ Future Work
- Implement **hyperparameter tuning** for DL models.
- Test on **real-time SMS datasets**.
- Explore other feature extraction methods like **Word Embeddings (Word2Vec, FastText, GloVe)**.



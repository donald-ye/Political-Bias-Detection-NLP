# 🧠 Political Bias & Misinformation Detection via NLP

## 📍 Problem Statement

We aim to investigate whether there is a correlation between **political bias** in text and the presence of **misinformation**.

Using **Twitter’s Community Notes** dataset and synthetically labeled political statements, we will:

- Detect political bias (from conservative to liberal) in text content using NLP techniques.
- Identify if politically biased content is correlated with misinformation.
- Cluster tweets based on learned political bias and misinformation labels to observe patterns.

---

## 🎯 End Goal

Produce a **clustering visualization** of tweets based on:

- **Political Bias**  
  - Encoded by color (e.g., red = liberal, blue = conservative)
- **Misinformation Status**  
  - Encoded by shape (e.g., triangle = misinformation, circle = factual)

> ⚠️ Note: The x- and y-axes represent abstract semantic embeddings, not literal political bias or misinformation scores.

---

## 🗂️ Dataset Overview

| Dataset Name                     | Purpose                          |
|----------------------------------|----------------------------------|
| `cajcodes/political-bias`        | Supervised political stance labels (0–4 scale) |
| `sweatSmile/news-sentiment-data` | News sentiment/bias analysis     |
| `strombergnlp/polstance`         | Stance classification            |
| **Twitter Community Notes**      | Real-world misinformation labels |

---

## 🧪 Methods

| Task                     | Data Type     | Approach        |
|--------------------------|---------------|------------------|
| Political Bias Detection | Labeled data  | Supervised ML (TF-IDF + DNN/LogReg) |
| Misinformation Detection | Weak labels   | Heuristic via Community Notes |
| Clustering               | TF-IDF vectors| Unsupervised (K-Means, t-SNE/UMAP) |
| Advanced Classification  | Tweet/news text| Transformers (BERT, RoBERTa, SimCSE) |

---

## 🔧 Pipeline Overview

1. **Preprocessing**  
   - Tokenization, cleaning, label standardization.
2. **Baseline Models**  
   - BoW + TF-IDF + Logistic Regression or DNN.
3. **Misinformation Detection**  
   - Use Community Notes as weak supervision.
4. **Clustering & Visualization**  
   - K-Means on TF-IDF vectors.
   - t-SNE/PCA/UMAP for 2D projection.
5. **Advanced Models**  
   - Fine-tune BERT/RoBERTa for bias detection.
   - SimCSE for embedding comparison.
6. **Evaluation**  
   - Accuracy, Precision, Recall, F1, ROC-AUC, Clustering Quality.
7. **Final Output**  
   - Visualization plots, confusion matrices, and performance summary.

---

## 📅 Weekly Plan

### Week 1: Mar 28 – Apr 3
- Select and explore datasets from Hugging Face.

### Week 2: Apr 4 – Apr 10
- Preprocess text and implement baseline TF-IDF + DNN/LogReg model.

### Week 3: Apr 11 – Apr 17
- Parse Twitter Community Notes and label tweets with misinformation tags.

### Week 4: Apr 18 – Apr 24
- Perform clustering and visualization using TF-IDF and dimensionality reduction.

### Week 5: Apr 25 – Apr 29
- Fine-tune transformer models, apply SimCSE, and complete model evaluation.

---

## 📌 Important Notes

- **Avoid labeling normative claims** (e.g., "Israel has the right to defend itself") as misinformation.
- Focus on **verifiable claims** (e.g., statistics, policy facts, historical dates).
- Be cautious about dataset generalizability:
  - Synthetic datasets may not include modern slang or key geopolitical issues.
  - Transformer models like BERT can help generalize across unseen topics.

---

## 🧾 Example Labels

| Text Snippet                                      | Likely Bias  | Notes                               |
|--------------------------------------------------|--------------|-------------------------------------|
| “Tax the rich.”                                  | Liberal (4)  | Left economic policy                |
| “Protect the Second Amendment.”                  | Conservative (0) | Right-leaning policy stance         |
| “Free Palestine and end the occupation.”         | Liberal      | Activist, anti-interventionist tone|
| “Strong national defense is our priority.”       | Conservative | Emphasis on military strength       |

---

## 🧩 Technologies Used

- **Python**, **TensorFlow**, **Scikit-learn**
- **Hugging Face Transformers & Datasets**
- **t-SNE**, **PCA**, **UMAP**, **K-Means**
- **Matplotlib**, **Seaborn**, **Plotly**

---

## ✅ Final Deliverables

- 📊 Bias vs. Misinformation Clustering Plot  
- 🤖 Final Trained Models (DNN, BERT/RoBERTa, SimCSE)  
- 📈 Evaluation Metrics + Visualizations  
- 📄 Final Report in `/docs/final_report.md`  
- 🧼 Clean, runnable GitHub repo with `README.md`

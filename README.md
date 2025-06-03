# 🗳️ Political Bias & Misinformation Detection | NLP & ML

This project uses Natural Language Processing (NLP) and Machine Learning (ML) to detect political bias in news articles and investigate its correlation with misinformation. It includes both **supervised classification** and **unsupervised clustering**, with a focus on **explainability**, **embedding quality**, and **ideological pattern discovery**.

---

## 📌 Project Highlights

- 🔍 **Fine-tuned BERT and SimCSE** for **multi-class political bias classification** (`left`, `center`, `right`) on a dataset of **34,000+ news articles**, achieving robust accuracy and semantic alignment.
  
- 🧠 Built **Logistic Regression** and **Deep Neural Networks** on **TF-IDF** and **Bag-of-Words** features:
  - Implemented **multi-layer ReLU architectures**
  - Used **dropout** for regularization and **categorical cross-entropy loss** for training
  - Provided baselines for transformer comparison

- 🧭 Applied **K-Means** and **HDBSCAN** to **transformer-based sentence embeddings**:
  - Discovered latent ideological clusters
  - Explored potential links between **political bias and misinformation patterns**
  - Enabled exploratory visualizations for further analysis

---

## 🧪 Technologies Used

| Category | Tools |
|---------|-------|
| NLP Models | BERT, SimCSE (Hugging Face Transformers) |
| ML Models | Logistic Regression, DNN (TensorFlow / Keras) |
| Feature Engineering | TF-IDF, Bag-of-Words |
| Clustering | K-Means, HDBSCAN |
| Evaluation | F1 Score, ROC-AUC, Cluster Consistency |
| Explainability | LIME, SHAP (optional extension) |

---

## 📁 Repository Structure

```plaintext
political-bias-detection/
├── data/                  # Processed & raw datasets
├── models/
│   ├── bert_finetune.py
│   ├── simcse_classify.py
│   ├── tfidf_dnn.py
│   └── logreg_baseline.py
├── clustering/
│   ├── kmeans_clusters.py
│   └── hdbscan_clusters.py
├── notebooks/
│   ├── exploratory_visuals.ipynb
│   └── embedding_evaluation.ipynb
├── requirements.txt
└── README.md

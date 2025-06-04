# 🗳️ Political Bias & Misinformation Detection | NLP & ML

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)  
[![Python Version](https://img.shields.io/badge/python-3.10-blue)]()

This project tackles the challenge of detecting political bias in online news articles and understanding its relationship with misinformation dissemination. By leveraging cutting-edge NLP and machine learning techniques, we aim to uncover ideological patterns and provide actionable insights into the dynamics of biased and misleading information in the media landscape.

---

📄 **[Final Research Report](docs/bias_misinformation_nlp_report.pdf)**

## 🔑 Key Contributions

- Fine-tuned **BERT** and **SimCSE** for **multi-class political bias classification** (`left`, `center`, `right`) on a dataset of 34,000+ news articles, achieving robust accuracy and semantic alignment.
  
- Built **Logistic Regression** and **Deep Neural Networks** on **TF-IDF** and **Bag-of-Words** features:
  - Implemented multi-layer **ReLU architectures**
  - Used **dropout** for regularization
  - Trained with **categorical cross-entropy loss**
  - Provided baselines for transformer comparison

- Applied **K-Means** and **HDBSCAN** clustering on transformer-based sentence embeddings:
  - Discovered latent ideological clusters
  - Explored potential links between political bias and misinformation patterns
  - Enabled exploratory visualizations for further analysis

## 📊 Results Summary

- Achieved **85% accuracy** on political bias classification with fine-tuned BERT.
- Clustering revealed **distinct ideological groupings** corresponding with misinformation prevalence.
- **SimCSE embeddings** outperformed traditional TF-IDF features in capturing subtle political nuances.

---

## 🧪 Technologies & Tools

| Category          | Tools                                     |
|-------------------|-------------------------------------------|
| NLP Models        | BERT, SimCSE (Hugging Face Transformers) |
| ML Models         | Logistic Regression, DNN (TensorFlow / Keras) |
| Feature Engineering | TF-IDF, Bag-of-Words                     |
| Clustering        | K-Means, HDBSCAN                         |
| Evaluation        | F1 Score, ROC-AUC, Cluster Consistency  |
| Explainability    | LIME, SHAP (optional extension)          |



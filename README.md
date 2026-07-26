# Explainable Email Spam and Phishing Detection System Based on a Transformer–XGBoost Hybrid Framework

## Overview

This repository contains the source code, experimental artefacts, and dissertation developed for my MSc research on **Explainable Artificial Intelligence (XAI) for Email Spam and Phishing Detection**.

The research proposes a hybrid machine learning framework that combines the contextual language understanding of Transformer models (BERT and RoBERTa) with the classification capability of XGBoost. To improve transparency and trustworthiness, the framework integrates SHAP and LIME for global and local model explanations.

---

## Research Objectives

The objectives of this research are to:

- Investigate existing approaches to email spam and phishing detection.
- Develop a Transformer–XGBoost hybrid detection framework.
- Compare the performance of BERT and RoBERTa.
- Integrate Explainable AI techniques (SHAP and LIME).
- Evaluate the effectiveness of the proposed framework using benchmark datasets.

---

## Proposed Framework

```text
Email
    │
    ▼
Data Preprocessing
    │
    ▼
Transformer Model
(BERT / RoBERTa)
    │
    ▼
Contextual Embeddings
([CLS] Representation)
    │
    ▼
XGBoost Classifier
    │
    ▼
Prediction
    │
    ▼
SHAP + LIME Explanations
```

---

## Repository Structure

```text
.
├── dissertation/          # LaTeX dissertation source
├── datasets/              # Dataset structure and download instructions
├── notebooks/             # Jupyter notebooks
├── models/                # Saved models (not tracked)
├── results/               # Experimental outputs
├── docs/                  # Supporting documentation
├── requirements.txt
├── LICENSE
├── .gitignore
└── README.md
```

---

## Technologies Used

- Python
- Jupyter Notebook
- PyTorch
- Hugging Face Transformers
- Scikit-learn
- XGBoost
- SHAP
- LIME
- Pandas
- NumPy
- Matplotlib

---

## Datasets

The experiments were conducted using publicly available benchmark datasets:

- SpamAssassin Public Corpus
- CEAS 2008 Spam Dataset
- Enron Email Dataset

The datasets are **not included** in this repository because of their size and licensing restrictions.

Instructions for downloading and preparing the datasets are available in:

```
datasets/README.md
```

---

## Experimental Workflow

1. Data collection
2. Data preprocessing
3. Fine-tuning BERT
4. Fine-tuning RoBERTa
5. Hybrid Transformer–XGBoost training
6. Model evaluation
7. Explainability analysis using SHAP
8. Explainability analysis using LIME
9. Comparative performance analysis

---

## Results

The proposed framework achieved excellent performance in detecting spam and phishing emails.

The evaluation includes:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve
- Precision–Recall Curve
- SHAP Feature Importance
- SHAP Force Plots
- LIME Local Explanations

Detailed results are available in the dissertation and the `results/` directory.

---

## Dissertation

The complete MSc dissertation is located in:

```
dissertation/
```

It includes:

- Chapter 1 – Introduction
- Chapter 2 – Literature Review
- Chapter 3 – Methodology
- Chapter 4 – Experimental Results and Discussion
- Chapter 5 – Conclusion and Recommendations

---

## Reproducing the Experiments

### Clone the repository

```bash
git clone https://github.com/<oluchukwuwalter>/<explainable email spam detection system>.git
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Download the datasets

Follow the instructions in:

```
datasets/README.md
```

### Run the notebooks

Execute the notebooks in numerical order:

1. Data preprocessing
2. BERT training
3. RoBERTa training
4. Hybrid model training
5. Evaluation
6. SHAP analysis
7. LIME analysis

---

## Future Work

Potential extensions of this research include:

- Evaluation using real-world enterprise email traffic
- Deployment as a real-time email filtering service
- Investigation of newer Transformer architectures
- Integration of multimodal phishing features
- Continual learning for evolving phishing attacks

---

## Author

**Walter Oluchukwu Ugwueze**
**Dike, Amaka Mercy**
**Olakanmi, Sola Alade**
**Taiwo, Nurudeen Olajide**

MSc Information Technology with Data Analytics  
University of the West of Scotland

Research Interests:

- Artificial Intelligence
- Explainable AI
- Machine Learning
- Natural Language Processing
- Cybersecurity
- Data Analytics

---

## License

This project is released under the MIT License.

---

## Citation

If you use this work in your research, please cite the accompanying MSc dissertation.

# aristia_ps4_ethics-and-algorithmic-bias 
**Dataset Used:** [Jigsaw Toxic Comment Classification Challenge — Kaggle](https://www.kaggle.com/datasets/julian3833/jigsaw-toxic-comment-classification-challenge?select=train.csv)
---
**Colab Notebook Link:** [COLAB NOTEBOOK](https://colab.research.google.com/drive/1Mv-P-HHcmCNfXr9ZRIOWdRft6dAtMP86?usp=sharing)
---

## 📌 About the Project

This project solves the problem of **bias in AI-generated content**.

It can:
- Detect biased or toxic text
- Explain why it is harmful
- Suggest a fair (debiased) version

---

## 🧠 How It Works

User gives text → Model analyzes → Output shows:
- Bias Score
- Explanation
- Debiased text

---

## 🤖 Model

- Model: DistilBERT (`distilbert-base-uncased`)
- Framework: PyTorch + HuggingFace
- Task: Text Classification (Biased / Fair)

---

## 📈 Results
The model was evaluated on **1000 test samples**.

### Overall Performance
| Metric | Score |
|--------|------|
| Accuracy | **95.80%** |
| Macro F1 Score | **0.89** |
| Weighted F1 Score | **0.96** |

---

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|------|-----------|--------|----------|---------|
| Fair (0) | 0.98 | 0.97 | 0.98 | 894 |
| Biased (1) | 0.79 | 0.83 | 0.81 | 106 |

---

### Confusion Matrix

|                | Predicted Fair | Predicted Biased |
|----------------|---------------|------------------|
| **Actual Fair**   | 870 | 24 |
| **Actual Biased** | 18  | 88 |

---


## ⚙️ How to Run

### 1. Clone repository and Download dataset from above link
```bash
git clone https://github.com/anmolbatra2005/aristia_ps4_ethics-and-algorithmic-bias.git
cd aristia_ps4_ethics-and-algorithmic-bias

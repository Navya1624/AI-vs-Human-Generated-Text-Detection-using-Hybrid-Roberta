# 🧠 AI Text Detection using Hybrid RoBERTa-BiLSTM Architecture

## 📌 Overview

This project focuses on detecting AI-generated text in academic writing using a **Hybrid Multi-Modal Deep Learning Architecture**.
The model combines **semantic understanding**, **sequential modeling**, and **linguistic stylometry** to improve detection accuracy and reduce false positives.

---

## 🚀 Key Features

* 🔹 Fine-tuned **RoBERTa** for contextual embeddings
* 🔹 **BiLSTM** for capturing sequential dependencies
* 🔹 **Attention Mechanism** for highlighting important tokens
* 🔹 **Stylometric Features (POS Density)** for structural analysis
* 🔹 Hybrid fusion of **semantic + syntactic features**

---

## 🏗️ Model Architecture

The proposed architecture follows a hybrid pipeline:

```
Input Text → RoBERTa → BiLSTM → Attention → Feature Fusion (POS) → Fully Connected Layer → Output (Human / AI)
```

---

## 📊 Datasets Used

* **DAIGT-V4 (Kaggle)** – Primary dataset (balanced 50K samples)
* **LLM Detect AI Text (Kaggle)** – Benchmark dataset
* **AI Text Detection Pile (HuggingFace)** – Large-scale diverse dataset

---

## 📈 Results

| Model                         | Accuracy | Precision | Recall   | F1-Score |
| ----------------------------- | -------- | --------- | -------- | -------- |
| Logistic Regression           | 0.87     | 0.86      | 0.87     | 0.86     |
| Fine-Tuned BERT               | 0.89     | 0.80      | 0.98     | 0.88     |
| **Hybrid RoBERTa (Proposed)** | **0.93** | **0.93**  | **0.92** | **0.93** |

✅ The hybrid model significantly reduces **False Positives (~65% reduction)** compared to BERT.

---

## 📉 Key Insight

* **BERT** → Highly sensitive (low FN, high FP)
* **Hybrid Model** → Balanced & precise (low FP, high reliability)

---

## 🧪 Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1-Score
* Confusion Matrix
* ROC-AUC Curve
* McNemar’s Test (Statistical Significance)

---

## ⚙️ Tech Stack

* Python
* PyTorch
* HuggingFace Transformers
* Scikit-learn
* Pandas / NumPy
* Google Colab (T4 GPU)

---

## ⏱️ Training Details

* GPU: NVIDIA Tesla T4 (16GB VRAM)
* BERT Training Time: ~22 mins/epoch
* Hybrid Model Training Time: ~40 mins/epoch

---


## ▶️ How to Run

1. Clone the repository

```
git clone https://github.com/your-username/AI-Text-Detection.git
```

2. Open notebook in Google Colab or Jupyter

3. Install dependencies

```
pip install -r requirements.txt
```

4. Run all cells

---

## 🔮 Future Work

* Explainable AI (SHAP, LIME)
* Multilingual detection
* Adversarial robustness (paraphrased AI text)
* Real-time deployment (API / Browser Extension)

---

## 📌 Conclusion

This project demonstrates that combining **semantic context with syntactic features** results in a more reliable AI-text detection system.
The proposed hybrid architecture achieves **high precision**, making it suitable for real-world academic applications.

---


Give this repo a ⭐ and share your feedback!

# Indonesian Batik Classification with DINOv3 🎨

**Fine-Grained Batik Motif Classification Using Self-Supervised Visual Features**

This project explores Indonesian batik motif classification using DINOv3, a self-supervised vision foundation model.

Instead of training a conventional classification head, the system extracts visual representations from images and performs similarity-based classification using K-Nearest Neighbors (KNN) and FAISS.

## ✨ Methodology

1. Dataset preparation and labeling.
2. Stratified Group K-Fold validation to reduce data leakage between related image groups.
3. DINOv3 feature extraction using a pretrained Vision Transformer.
4. Feature representation through token pooling.
5. Similarity search using FAISS.
6. Classification using K-Nearest Neighbors and cosine similarity.
7. Model evaluation.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Feature Extractor:** DINOv3 Base
- **Deep Learning:** PyTorch
- **Similarity Search:** FAISS
- **Classification:** K-Nearest Neighbors
- **Data Processing:** NumPy, Pandas
- **Evaluation:** Scikit-learn

## 🏗️ System Architecture

```text
Batik Image Dataset
        |
        v
Dataset Preparation
        |
        v
Stratified Group K-Fold
        |
        v
Pretrained DINOv3
        |
        v
Feature Extraction
        |
        v
Feature Embeddings
        |
        v
FAISS Similarity Search
        |
        v
KNN Classification
        |
        v
Evaluation Results
```

## 📊 Dataset

- Total images: 1,500
- Number of classes: 10
- Classification task: Indonesian batik motif recognition

## 📈 Experimental Results

- Global Accuracy: **94.60%**

> This value represents the reported experimental result. Add the evaluation protocol, per-fold metrics, confusion matrix, and other metrics to make the result reproducible and interpretable.

## 🎯 Research Objectives

- Explore self-supervised visual representations for fine-grained image classification.
- Evaluate DINOv3 embeddings for Indonesian batik motif recognition.
- Investigate similarity-based classification without conventional end-to-end classifier training.
- Support the documentation and preservation of Indonesian cultural heritage.

## 🔬 Key Research Components

- Self-supervised learning.
- Vision Transformer.
- Feature embedding extraction.
- Cosine similarity.
- Approximate nearest neighbor search.
- Group-aware cross-validation.

## 🚀 Getting Started

Install the required dependencies:

```bash
pip install torch torchvision
pip install faiss-cpu
pip install numpy pandas scikit-learn
```

> Add the exact DINOv3 installation procedure, pretrained checkpoint acquisition instructions, and experiment commands used in this repository.

## 📚 Research Status

This repository contains the implementation and experimental work for an Indonesian batik motif classification study.

[TODO: Add publication information or manuscript link when available.]

## 👨‍💻 Author

Developed by **Nazril Hidayatulloh**.

---

*Exploring self-supervised learning for Indonesian cultural heritage preservation.*

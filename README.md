# Breast Ultrasound Lesion Classification (BUSI Dataset)

**Students:** José Tuozzo  
**Course:** ITAI 1378 — Computer Vision & AI  
**Project Tier:** Tier 2 — Applied Medical CV Project  

---

## 🚀 Project Overview

Breast cancer is one of the leading causes of death among women worldwide.  
Ultrasound imaging is a common diagnostic tool, yet interpretation accuracy can vary across clinicians and small tumors can be missed.

This project builds a **computer vision model using deep learning** to classify breast ultrasound images as **Benign vs Malignant** and generate **Grad-CAM heatmaps** for transparency.

⚠️ *This is a learning prototype for educational purposes only — not for clinical use.*

---

## 🎯 Project Objectives

| Goal | Description |
|---|---|
| Image Classification | Detect *Benign vs Malignant* lesions |
| Explainability | Grad-CAM heatmaps for medical interpretability |
| Efficiency | Transfer learning for fast training |
| Practicality | Real-world clinical support scenario (triage tool) |

---

## 🧠 Technical Approach

| Component | Decision |
|---|---|
Task | Binary image classification  
Model | Transfer learning (ResNet-50 / EfficientNet-B0)  
Framework | PyTorch + Torchvision  
Canvas/Compute | Google Colab  
Explainability | Grad-CAM integration  
Data Split | 70% train • 15% validation • 15% test  

**Why this approach?**  
Transfer learning gives strong performance with limited medical data while remaining computationally feasible for a student prototype.

---

## 📦 Dataset

**BUSI — Breast Ultrasound Images Dataset**  
Source: Kaggle  
Total images: ~780  
Classes used: **Benign vs Malignant**

Preprocessing:

- Resize → 224×224
- Normalize (ImageNet)
- Data augmentation (flip, rotation, brightness)
- Class imbalance handling

Dataset link: *(add after download)*

---

## 📈 Evaluation Metrics

| Metric | Target |
|---|---|
Accuracy | ≥ 90%  
Precision/Recall | ≥ 88%  
Explainability | Meaningful heatmaps for tumor localization  
Latency | < 1s per image (CPU)  

---

## 📅 Timeline

| Week | Task | Deliverable |
|---|---|---|
Week 10 | Dataset setup, notebook structure | Ready environment  
Week 11 | Training & fine-tuning | Base model trained  
Week 12 | Evaluation & Grad-CAM | Results + heatmaps  
Week 13 | Demo + video | Working demo  
Week 14 | Docs + README polish | Submission-ready repo  
Week 15 | Final presentation | 🎤 In-class presentation  

---

## ⚠️ Risks & Mitigation

| Risk | Probability | Mitigation |
|---|---|---|
Class imbalance | Medium | Class weights, augmentation |
Limited data | High | Augmentation, Kaggle alt datasets |
Training instability | Low | Early stopping, LR scheduling |
Low accuracy | Medium | Try EfficientNet, tune LR/epochs |

---

## 🧰 Tools & Resources

- Google Colab
- Python 3.10
- PyTorch / Torchvision
- OpenCV
- Matplotlib
- Grad-CAM Library

Cost: **$0**

---

## 🙌 AI Usage Log

AI tools (ChatGPT) used to:

- Refine project proposal language
- Generate README structure
- Provide initial notebook skeleton

Model training, coding, and evaluation will be self-implemented.

---

## 📎 Folder Structure

project/
├── README.md
├── requirements.txt
├── notebooks/
│ └── 01_exploration.ipynb
├── data/
│ └── README.md
└── docs/
└── proposal.pdf

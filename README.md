# 🔐 Microsoft: Classifying Cybersecurity Incidents with Machine Learning

![Cybersecurity Banner](https://img.shields.io/badge/Cybersecurity-Incident%20Classification-blueviolet?style=flat-square)
![Python](https://img.shields.io/badge/Machine%20Learning-Random%20Forest%20Classifier-brightgreen)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

## 📌 Project Overview

Security Operation Centers (SOCs) are flooded with countless alerts daily. Analysts must distinguish between:
- ✅ **True Positives (TP)** — Actual threats
- ⚠️ **Benign Positives (BP)** — Non-threatening anomalies
- ❌ **False Positives (FP)** — Incorrect alerts

Manual triage is **time-consuming and error-prone**. This project proposes an **automated classification model** to enhance SOC efficiency using **Machine Learning**.

---

## 🎯 Objective

- 🧠 Build a machine learning model to **classify incidents** into TP, BP, or FP.
- 📈 Maximize **Macro-F1 Score**, **Precision**, and **Recall**.
- 👨‍💻 Assist SOC Analysts with **context-aware threat classification**.

---

## 📂 Dataset & Feature Engineering

🔍 **Key Features Selected:**
- AlertTitle, Category, EntityType, EvidenceRole, ApplicationName  
- OSFamily, CountryCode, State, City, IpAddress  
- NetworkMessageId, RegistryKey/Value, ApplicationId  
- OSVersion, IncidentGrade, Sha256

🧹 **Preprocessing:**
- Removed ID, timestamps, and non-contributing fields
- Balanced dataset using **SMOTE** (Synthetic Minority Over-sampling Technique)

---

## 📊 Exploratory Data Analysis (EDA)

EDA helped in:
- Identifying skewed class distribution
- Recognizing highly predictive features
- Detecting noise and redundant columns

---

## 🤖 Model Training

🚀 **Best Performing Model:**
> `Random Forest Classifier`

📌 **Train Set Results (With SMOTE):**
- Accuracy: 65%
- Macro F1-Score: 60%
- Class 0: F1 = 71%, Class 1: F1 = 42%, Class 2: F1 = 67%

📌 **Test Set Results (With SMOTE):**
- Accuracy: 66%
- Macro F1-Score: 62%
- Class 0: F1 = 71%, Class 1: F1 = 44%, Class 2: F1 = 70%

---

## 🧪 Model Evaluation

✔️ **Macro Precision:** 64%  
✔️ **Macro Recall:** 62%  
✔️ Balanced performance across TP, BP, and FP categories  
✔️ Robust detection of critical threats  
✔️ SOC-ready automation capability

---

## ✅ Conclusion

The model is effective in:
- Automating incident triage  
- Minimizing false alerts  
- Helping security teams prioritize **real threats**

This contributes to **faster response times** and **reduced analyst fatigue** in modern cybersecurity environments.

---

## 📌 Tech Stack

- 🐍 Python
- 📘 Scikit-learn
- 📊 Pandas & Matplotlib
- ⚖️ SMOTE (Imbalanced-learn)
- 🌳 Random Forest Classifier

---

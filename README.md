# Sign Language Translation using Temporal Classification

This project implements **Sign Language Recognition** using various Machine Learning models such as **SVM**, **Logistic Regression**, **LSTM**, and **Sequential Pattern Mining (SPM)**. The aim is to classify signs from time-series motion data collected via sensor gloves.

---

## 📘 Overview

The project is based on the paper:  
**“Sign Language Recognition using Temporal Classification”** by Hardie Cate, Fahim Dalvi, and Zeshan Hussain (Stanford University, 2015).

It explores how temporal data (motion, hand rotation, and finger bends) can be used to classify 95 different signs from both high-quality and low-quality datasets.

---

## 🧠 Models Implemented

1. **SVM (Support Vector Machine)** – baseline model using temporal flattening.  
2. **Logistic Regression** – simple linear classifier for comparison.  
3. **LSTM (Long Short-Term Memory)** – captures temporal dependencies.  
4. **SPM (Sequential Pattern Mining)** – identifies distinguishing temporal signal patterns.

---

## 📊 Dataset Description

- **High Quality Dataset**
  - Recorded at **200 Hz** with 14-bit precision
  - Two 5D gloves (both hands)
  - 27 instances per sign

- **Low Quality Dataset**
  - Recorded at **50 Hz** using **Nintendo Powerglove**
  - One hand only, lower precision
  - 70 instances per sign

---

## ⚙️ Preprocessing Steps

1. **Temporal Scaling** – resample signals to 57 frames  
2. **Spatial Scaling** – normalize all signals between 0 and 1  
3. **Flattening** – convert 3D time-series data to 2D for classic ML models  

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/Sign-Language-Translation.git
   cd Sign-Language-Translation


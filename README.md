# Transformer Fault Prediction using Machine Learning

A Machine Learning based system for predicting faults in distribution transformers using thermal, voltage, and current parameters.

## 📌 Project Overview

Transformers are important components of electrical power distribution systems. Unexpected transformer faults can lead to equipment damage, power interruptions, and increased maintenance costs.

This project uses Machine Learning classification algorithms to analyze transformer operating parameters and predict the **Magnetic Oil Gauge (MOG_A)** fault indicator.

The project also provides a Streamlit-based web application where transformer parameters can be entered and the prediction can be viewed through a simple user interface.

---

## 🎯 Objectives

- Analyze transformer operating data.
- Perform Exploratory Data Analysis (EDA).
- Clean and merge transformer datasets.
- Visualize important parameters.
- Train multiple Machine Learning classification models.
- Compare the performance of different models.
- Develop a simple web interface for transformer fault prediction.

---

## ⚙️ Input Parameters

The prediction system uses 16 transformer parameters.

### Thermal Parameters

| Parameter | Description |
|---|---|
| OTI | Oil Temperature Indicator |
| WTI | Winding Temperature Indicator |
| ATI | Ambient Temperature Indicator |
| OLI | Oil Level Indicator |
| OTI_A | Oil Temperature Indicator Alarm |
| OTI_T | Oil Temperature Indicator Trip |

### Electrical Parameters

| Parameter | Description |
|---|---|
| VL1 | Phase 1 Voltage |
| VL2 | Phase 2 Voltage |
| VL3 | Phase 3 Voltage |
| IL1 | Phase 1 Current |
| IL2 | Phase 2 Current |
| IL3 | Phase 3 Current |
| VL12 | Line Voltage 1-2 |
| VL23 | Line Voltage 2-3 |
| VL31 | Line Voltage 3-1 |
| INUT | Neutral Current |

### Target

**MOG_A — Magnetic Oil Gauge Indicator**

---

## 🤖 Machine Learning Models

The project implements and compares multiple classification algorithms:

- Logistic Regression
- Support Vector Classifier (SVC)
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Extra Trees
- AdaBoost
- XGBoost

The predictions from the trained models are used to determine the transformer fault risk.

---

## 🔄 Project Workflow

```text
Transformer Dataset
        ↓
Data Loading
        ↓
Data Cleaning & Preprocessing
        ↓
Exploratory Data Analysis
        ↓
Feature Selection
        ↓
Train-Test Split
        ↓
Data Normalization
        ↓
Machine Learning Models
        ↓
Model Evaluation
        ↓
Fault Prediction
        ↓
Streamlit Web Application

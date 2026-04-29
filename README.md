# 🚨 Network Intrusion Detection System (IDS)

## 📌 Overview

This project focuses on building a Machine Learning-based Intrusion Detection System to identify malicious network activity and classify different types of cyber-attacks.

---

## 🎯 Objectives

* Perform **Binary Classification** (Normal vs Attack)
* Perform **Multiclass Classification** (Identify specific attack types)
* Handle **imbalanced dataset**
* Evaluate model performance using appropriate metrics

---

## 📊 Dataset

The dataset contains network traffic features such as:

* Duration, protocol type, service, flag
* Source & destination bytes
* Error rates and connection statistics

⚠️ Note: Dataset is not included due to large size.

---

## ⚙️ Approach

### 1. Data Preprocessing

* Combined multiple attack datasets
* Removed corrupted columns (e.g., 0.23, 0.24)
* Handled missing values
* Encoded categorical variables

---

### 2. Models Used

* Logistic Regression
* Random Forest Classifier

---

## 📈 Results

### 🔹 Binary Classification

* Accuracy: ~99.9%
* Successfully detects whether traffic is normal or malicious

### 🔹 Multiclass Classification

* Accuracy: ~99.9%
* Strong performance on major classes
* Lower performance on rare attack types due to class imbalance

---

## ⚠️ Key Insight

The dataset is highly imbalanced. Rare attack types like:

* FTPWrite
* RootKit
* BufferOverflow

have very few samples, making them difficult to predict accurately.

---

## 📂 Repository Structure

* `intrusion_detection_model.ipynb` → Main notebook
* `binary_predictions.csv` → Binary classification results
* `multiclass_predictions_readable.csv` → Multiclass results

---

## 🚀 Conclusion

Binary classification performs extremely well, while multiclass classification provides deeper insights but is affected by class imbalance. Random Forest outperformed Logistic Regression in this project.

---

## 👨‍💻 Author

Aditya Singh

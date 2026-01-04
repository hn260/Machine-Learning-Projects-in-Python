# 🚗 Car Price Prediction Model

---

## 📌 Project Overview

This repository demonstrates a **clean, reproducible workflow** for building and running a **Car Price Prediction model** using datasets sourced directly from **Kaggle inside Google Colab**, without downloading anything locally.

The focus is on **proper ML workflow hygiene**: reproducibility, clean data access, and separation of code and data.

---

## 🛠 Technologies Used

* Python
* Google Colab
* Kaggle API
* Jupyter Notebook

---

## 🚀 Key Capabilities

* Load Kaggle datasets directly into Colab
* Avoid local dataset downloads and manual uploads
* Maintain reproducible ML experiments
* Optional persistent storage using Google Drive
* Keep GitHub repositories clean and lightweight

---

## 🔄 Process & Workflow

### 1️⃣ Kaggle API Authentication

* Generate `kaggle.json` from Kaggle account
* Upload credentials securely to Colab
* Configure permissions for API access

### 2️⃣ Dataset Download via Kaggle API

* Identify the dataset slug from Kaggle
* Download dataset programmatically
* Extract files automatically into the runtime

### 3️⃣ Optional Persistent Storage

* Mount Google Drive for session persistence
* Store datasets without committing them to GitHub

---

## 🧠 What I Learned

* How to integrate Kaggle datasets directly into Colab
* Why reproducibility matters in ML projects
* Secure handling of API credentials
* Keeping repositories professional and uncluttered
* Treating datasets as dependencies, not source code

---

## 📈 Overall Growth

This project reinforced:

* An engineering-first ML mindset
* Cleaner experiment setup and iteration
* Better separation of data, configuration, and logic
* Industry-aligned ML project practices

---

## 🔧 Possible Improvements

* Dataset versioning support
* Config-driven dataset selection
* Experiment tracking integration
* Automated validation after data loading

---

## ▶️ How to Run the Project

### 1️⃣ Install Kaggle API

```python
!pip install kaggle
```

### 2️⃣ Upload Kaggle Credentials

```python
from google.colab import files
files.upload()
```

Upload `kaggle.json`.

---

### 3️⃣ Configure API Access

```python
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json
```

---

### 4️⃣ Download Dataset

```python
!kaggle datasets download -d <dataset-owner>/<dataset-name>
!unzip <dataset-name>.zip
```

---

### (Optional) Persistent Storage

```python
from google.colab import drive
drive.mount('/content/drive')
```


# 📊 Machine Learning Models Portfolio

---

## 📌 Repository Overview

This repository contains a **curated collection of machine learning models** built to solve a variety of **real-world prediction and classification problems**.

The focus across all projects is not just model accuracy, but **clean ML workflows**, **reproducibility**, and **engineering discipline** — from dataset ingestion to evaluation.

All models follow a **consistent structure and methodology**, making this repository easy to navigate, understand, and extend.

---

## 🧠 Problems Covered

The models in this repository span multiple domains:

* **Regression**

  * Car Price Prediction
  * House Price Prediction
  * Wine Quality Prediction

* **Classification**

  * Customer Churn Prediction
  * Titanic Survival Prediction

* **Healthcare & Medical**

  * Heart Disease Prediction
  * Diabetes Prediction
  * Autism Prediction

Each notebook focuses on **one well-defined problem**, avoiding unnecessary scope creep.

---

## 🛠 Technologies Used

* Python
* Google Colab
* Kaggle API
* Jupyter Notebook
* NumPy, Pandas, Scikit-learn

---

## 🔄 Standard Workflow (Used Across All Models)

Every project in this repository follows the same disciplined pipeline:

1. **Dataset Integration**

   * Datasets sourced from Kaggle
   * Downloaded programmatically using the Kaggle API
   * No raw datasets committed to the repository

2. **Data Preparation**

   * Cleaning and preprocessing
   * Handling missing values and outliers
   * Feature encoding and scaling

3. **Model Development**

   * Algorithm selection based on problem type
   * Model training and evaluation
   * Iterative refinement using appropriate metrics

4. **Evaluation & Analysis**

   * Task-relevant metrics (not just accuracy)
   * Clear separation of results and logic

This consistency ensures **reproducibility and clarity** across all experiments.

---

## 📁 Repository Structure

```
machine-learning-models/
│── Car Price Prediction Model.ipynb
│── House Price Prediction Model.ipynb
│── Wine Quality Prediction Model.ipynb
│── Customer Churn Prediction Model.ipynb
│── Titanic Survival Prediction Model.ipynb
│── Heart Disease Prediction Model.ipynb
│── Diabetes Prediction Model.ipynb
│── Autism Prediction Model.ipynb
│── README.md
```

(Each notebook has its own detailed README when viewed individually.)

---

## 🧠 What This Repository Demonstrates

* Strong fundamentals in machine learning workflows
* Clean, reproducible experimentation practices
* Ability to handle diverse datasets and problem types
* Consistency in structure and documentation
* An engineering-first approach to ML, not ad-hoc notebooks

---

## 📈 Overall Growth

Through these projects, I strengthened:

* End-to-end ML problem solving
* Dataset handling without repository pollution
* Model evaluation beyond surface-level metrics
* Discipline in structuring ML work professionally

This repository reflects **progression and consolidation**, not random experimentation.

---

## 🔧 Future Improvements

* Hyperparameter tuning and model comparison across projects
* Feature importance and interpretability analysis
* Model persistence and deployment pipelines
* Experiment tracking and benchmarking
* Migration of selected models to production-ready services

---

## ▶️ How to Run Any Model

1. Open the desired notebook in **Google Colab**
2. Set up Kaggle API access:

   ```python
   !pip install kaggle
   from google.colab import files
   files.upload()
   ```
3. Configure credentials:

   ```python
   !mkdir -p ~/.kaggle
   !cp kaggle.json ~/.kaggle/
   !chmod 600 ~/.kaggle/kaggle.json
   ```
4. Run the dataset download cell inside the notebook
5. Execute all cells top-to-bottom


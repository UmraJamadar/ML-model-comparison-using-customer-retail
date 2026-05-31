# 🛒 Customer Retail Dataset — ML Model Comparison

> **DevTown 5-Day Machine Learning Mastery Bootcamp Project**  
> Comparing Logistic Regression, Decision Tree & KNN on real-world retail data

---

## 📌 Project Overview

This project builds and compares three supervised Machine Learning classification models on the UCI Online Retail Dataset. Each transaction is classified as **High Value** or **Low Value** based on Quantity, UnitPrice, and Country.

---

## 🤖 Models Used

| Model | Description |
|---|---|
| Logistic Regression | Linear classifier, fast & interpretable baseline |
| Decision Tree (depth=5) | Non-linear splits, handles patterns well |
| KNN (k=7) | Distance-based, adapts to local clusters |

---

## 📊 Dataset Features

| Feature | Type | Description |
|---|---|---|
| Quantity | Integer | Units purchased per transaction |
| UnitPrice | Float | Price per unit (GBP) |
| Country | Categorical | Customer's country |
| HighValue *(engineered)* | Binary (0/1) | 1 if TotalAmount > median |

---

## 🗂️ Project Structure

```
📁 ML_Customer_Retail_Project/
├── ML_Customer_Retail_Project.ipynb   ← Main notebook (run this!)
├── README.md                          ← This file
├── customer_distribution.png          ← Generated after running
├── confusion_matrices.png             ← Generated after running
└── model_accuracy_comparison.png      ← Generated after running
```

---

## 🚀 How to Run

### Option 1 — Google Colab (Recommended)
1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Open Notebook → GitHub tab**
3. Paste your GitHub repo URL and open the `.ipynb` file
4. Click **Runtime → Run All**

### Option 2 — Local
```bash
git clone https://github.com/YOUR_USERNAME/ML_Customer_Retail_Project
cd ML_Customer_Retail_Project
pip install pandas scikit-learn matplotlib seaborn openpyxl
jupyter notebook ML_Customer_Retail_Project.ipynb
```

---

## 📈 Workflow

1. Load dataset (UCI Online Retail)
2. Handle missing values & remove invalid rows
3. Encode `Country` using LabelEncoder
4. Engineer `TotalAmount` and `HighValue` target
5. Visualise data (3 graphs)
6. Split data — 80% train / 20% test
7. Train Logistic Regression, Decision Tree, KNN
8. Evaluate with Accuracy Score + Confusion Matrix
9. Compare models with bar chart

---

## 🎓 Built During

**DevTown Machine Learning Mastery Bootcamp**  
📅 May 23–27, 2026 | 5 Days | 100% Online | Free

---

## 🛠️ Tech Stack

`Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn` `Jupyter Notebook`

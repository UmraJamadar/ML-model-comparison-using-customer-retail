# Customer Retail Dataset — ML Model Comparison

> **Machine Learning Project**  
> Comparing Logistic Regression, Decision Tree & KNN on real-world retail data

---

## 📌 Project Overview

This project builds and compares three supervised Machine Learning classification models on the UCI Online Retail Dataset. Each transaction is classified as **High Value** or **Low Value** based on Quantity, UnitPrice, and Country.

---

## Models Used

| Model | Description |
|---|---|
| Logistic Regression | Linear classifier, fast & interpretable baseline |
| Decision Tree (depth=5) | Non-linear splits, handles patterns well |
| KNN (k=7) | Distance-based, adapts to local clusters |

---

## Dataset Features

| Feature | Type | Description |
|---|---|---|
| Quantity | Integer | Units purchased per transaction |
| Price | Float | Price per unit (GBP) |
| Country | Categorical | Customer's country |
| HighValue *(engineered)* | Binary (0/1) | 1 if TotalAmount > median |

---

## Project Structure

```
📁 ML_Customer_Retail_Project/
├── ML_Customer_Retail_Project.ipynb   ← Main notebook (run this!)
├── README.md                          ← This file
├── customer_distribution.png          ← Generated after running
├── confusion_matrices.png             ← Generated after running
└── model_accuracy_comparison.png      ← Generated after running
```

---

## How to Run

### Option 1 — Google Colab (Recommended)
1. Go to [colab.research.google.com](https://colab.research.google.com)
2. Click **File → Open Notebook → GitHub tab**
3. Paste your GitHub repo URL and open the `.ipynb` file
4. Click **Runtime → Run All**

### Option 2 — Local
1. Clone the repo
2. Open the .ipynb file in VS Code
3. Install Jupyter extension in VS Code
4. Download the dataset from Kaggle:
   https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci
5. Place online_retail.xlsx in the same folder
6. Update the file path in Step 2 cell
7. Run All cells

## Workflow

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

## Tech Stack

`Python` `Pandas` `Scikit-learn` `Matplotlib` `Seaborn` `Jupyter Notebook`

# 🩺 Diabetes Dataset — Exploratory Data Analysis

[![Python](https://img.shields.io/badge/Python-3.13-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](#-license)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)](#)

Exploratory Data Analysis (EDA) on the Pima Indians Diabetes dataset to understand the factors associated with diabetes outcomes, using Python, Pandas, NumPy, Matplotlib, and Seaborn.

## 📖 Table of Contents

- [Project Overview](#-project-overview)
- [Objective](#-objective)
- [Dataset](#️-dataset)
- [Tools & Technologies](#️-tools--technologies)
- [Repository Structure](#-repository-structure)
- [Analysis Workflow](#-analysis-workflow)
- [Key Findings](#-key-findings)
- [Conclusion](#-conclusion)
- [Getting Started](#-getting-started)
- [Author](#-author)


## 📌 Project Overview

This project explores a diabetes dataset to uncover patterns, distributions, and relationships between health-related features and the diabetes outcome. The analysis covers:

- Dataset structure and data types
- Data cleaning and validation
- Statistical distributions and summaries
- Missing, duplicate, and zero-value analysis
- Outlier detection
- Relationships between variables
- Diabetes outcome analysis
- Actionable analytical insights

## 🎯 Objective

To explore the dataset and identify patterns and relationships between health-related features (glucose, BMI, age, pregnancies, etc.) and the diabetes outcome.

## 🗂️ Dataset

The dataset (`diabetes.csv`) contains **768 observations** and **9 variables**:

| Column | Description |
|---|---|
| `Pregnancies` | Number of times pregnant |
| `Glucose` | Plasma glucose concentration |
| `BloodPressure` | Diastolic blood pressure (mm Hg) |
| `SkinThickness` | Triceps skin fold thickness (mm) |
| `Insulin` | 2-Hour serum insulin (mu U/ml) |
| `BMI` | Body mass index |
| `DiabetesPedigreeFunction` | Diabetes pedigree function score |
| `Age` | Age in years |
| `Outcome` | Diabetes outcome (0 = non-diabetic, 1 = diabetic) |

**Source:** [Pima Indians Diabetes Database (Kaggle)](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database) — originally from the National Institute of Diabetes and Digestive and Kidney Diseases.

**View the data:**
- Open [`diabetes.csv`](./diabetes.csv) directly in this repository,
- 📓 View the notebook: [Diabetes Dataset — Exploratory Data Analysis.ipynb](./Diabetes%20Dataset%20—%20Exploratory%20Data%20Analysis.ipynb) or
- Load it in Python:


```python
import pandas as pd
df = pd.read_csv("diabetes.csv")
df.head()
```

## 🛠️ Tools & Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📁 Repository Structure

```
├── Diabetes_Dataset___Exploratory_Data_Analysis.ipynb   # Main analysis notebook
├── diabetes.csv                                          # Dataset
└── README.md
```

## 🔍 Analysis Workflow

The notebook walks through the following steps:

1. Import required libraries
2. Load the dataset
3. Dataset dimensions
4. Dataset columns
5. Dataset information
6. Statistical summary
7. Missing value analysis
8. Duplicate record analysis
9. Unique value analysis
10. Diabetes outcome distribution
11. Zero value analysis
12. Distribution of numerical variables
13. Outlier analysis
14. Correlation analysis
15. Glucose level vs. diabetes outcome
16. BMI vs. diabetes outcome
17. Age vs. diabetes outcome
18. Pregnancies vs. diabetes outcome
19. Glucose distribution by outcome
20. Multivariate relationship analysis
21. Outcome percentage analysis
22. Group-wise statistical analysis
23. Features most associated with outcome

## 📊 Key Findings

- The dataset contains **768 observations and 9 variables**, with **no explicit null values**.
- The `Outcome` variable is binary and **imbalanced**, with more non-diabetic than diabetic observations.
- Several medical variables (e.g., `Insulin`, `SkinThickness`, `BloodPressure`) contain **zero values** that likely represent missing data and warrant further investigation.
- **Glucose** shows the strongest positive correlation with diabetes outcome, followed by **BMI**, **Age**, and **Pregnancies**.
- BMI and Age distributions differ between outcome groups, though with substantial overlap.
- Several variables, particularly **Insulin**, contain potential outliers.
- Diabetes outcome appears to be associated with multiple variables rather than a single feature — correlation reflects association, not causation.

### Group-wise Averages (by Outcome)

| Outcome | Pregnancies | Glucose | BloodPressure | BMI | Age |
|---|---|---|---|---|---|
| 0 (Non-diabetic) | 3.30 | 109.98 | 68.18 | 30.30 | 31.19 |
| 1 (Diabetic) | 4.87 | 141.26 | 70.82 | 35.14 | 37.07 |

## 🏁 Conclusion

The EDA provides an overall understanding of the diabetes dataset, examining structure, data quality, distributions, outliers, correlations, and feature relationships. Glucose shows the most noticeable association with diabetes outcome, with BMI and age also contributing meaningful differences between groups. These findings highlight patterns worth further investigation but do not establish causal relationships. The cleaned and analyzed dataset provides a solid foundation for further statistical analysis or machine learning modeling.

## 🚀 Getting Started

### Prerequisites

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

### Run the notebook

```bash
git clone https://github.com/Soumya0006/<repo-name>.git
cd <repo-name>
jupyter notebook Diabetes_Dataset___Exploratory_Data_Analysis.ipynb
```

## 👤 Author

**Soumya Ranjan Das**

- GitHub: [@Soumya0006](https://github.com/Soumya0006)
- LinkedIn: [Soumya Ranjan Das](https://www.linkedin.com/in/soumya-ranjan-das-660a1140b)
- Email: [sd5916111@gmail.com](mailto:sd5916111@gmail.com)

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to check the [issues page](../../issues) or open a pull request.


## ⭐ Acknowledgements

- Dataset provided by the National Institute of Diabetes and Digestive and Kidney Diseases, hosted on Kaggle.
- Built with [Pandas](https://pandas.pydata.org/), [NumPy](https://numpy.org/), [Matplotlib](https://matplotlib.org/), and [Seaborn](https://seaborn.pydata.org/).

---

If you found this project useful, consider giving it a ⭐ on GitHub!

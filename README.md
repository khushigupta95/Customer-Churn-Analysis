# 📌 Customer Churn Analysis
**Analyzing customer churn patterns using Python for data preprocessing, analysis, and visualization.**

---

## 📂 Project Overview
This project focuses on understanding customer churn trends using Python. It involves **data cleaning, exploratory data analysis (EDA), and visualization** to derive insights that help improve customer retention.

---

## 📁 Files Included
- -<a href="https://github.com/khushigupta95/Customer-Churn-Analysis/blob/main/Customer%20Churn.csv">Dataset</a> - The dataset used for analysis.  
- -<a href="https://github.com/khushigupta95/Customer-Churn-Analysis/blob/main/TCA.ipynb">Jupyter notebook</a> - Exploratory Data Analysis (EDA) with visualizations.  
  
---

## 🛠️ Tools & Technologies Used
- **Python** (Pandas, NumPy, Matplotlib, Seaborn)

---

## 📌 Steps Followed

### 1️⃣ Data Loading
- Imported the dataset using Pandas:  
  ```python
  import pandas as pd  
  df = pd.read_csv('churn_data.csv')  
  df.head()

### 2️⃣ Data Cleaning & Preprocessing (Refer to eda.ipynb)
 - **Check for missing values**

   df.isnull().sum()

- **Drop missing values**

   df.dropna(inplace=True)

- **Convert categorical variables into numerical format**

  df['Churn'] = df['Churn'].map({'Yes': 1, 'No': 0})


### 3️⃣ Exploratory Data Analysis (EDA) (Refer to eda.ipynb)
- **Visualized churn distribution:**

 import seaborn as sns  
 import matplotlib.pyplot as plt  

- **Churn distribution**

 sns.countplot(x=df['Churn'])
 plt.show()
 
 ![Churned Customers by Payment Method](https://raw.githubusercontent.com/khushigupta95/Customer-Churn-Analysis/main/IMAGES/Screenshot%20(61).png)

![Multiple Countplots](https://raw.githubusercontent.com/khushigupta95/Customer-Churn-Analysis/main/IMAGES/Screenshot%20(62).png)

![Histogram of Tenure](https://raw.githubusercontent.com/khushigupta95/Customer-Churn-Analysis/main/IMAGES/Screenshot%20(63).png)

### 🎯 Conclusion

This project provides valuable insights into customer churn analysis using Python.  
By understanding key trends and visualizing churn patterns, businesses can develop  
better strategies to improve customer retention.  
Future work can include deeper analysis using machine learning models for predictions. 




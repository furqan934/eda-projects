# 🚢 Titanic Exploratory Data Analysis (EDA)

## 📌 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on the Titanic dataset to uncover patterns, relationships, and key factors that influenced passenger survival.

The analysis follows a structured data science workflow, including data cleaning, visualization, and interpretation, making it suitable for both learning and portfolio purposes.

---

## 🎯 Objective

* Understand the structure and quality of the dataset
* Perform data cleaning and preprocessing
* Analyze feature distributions and relationships
* Identify key factors affecting survival
* Generate meaningful insights for decision-making

---

## 📊 Dataset Information

* **Dataset:** Titanic (Kaggle)
* **Number of Rows:** 891
* **Number of Columns:** 12

### 🔑 Key Features:

* `Survived` → Target variable (0 = No, 1 = Yes)
* `Pclass` → Passenger class (1st, 2nd, 3rd)
* `Sex` → Gender
* `Age` → Age of passenger
* `Fare` → Ticket fare
* `SibSp` → Number of siblings/spouses aboard
* `Parch` → Number of parents/children aboard
* `Embarked` → Port of embarkation

---

## 🛠️ Technologies Used

* **Python**
* **Pandas** → Data manipulation
* **NumPy** → Numerical operations
* **Matplotlib** → Data visualization
* **Seaborn** → Statistical visualization

---

## 🔍 EDA Workflow

### 1️⃣ Data Loading & Understanding

* Loaded dataset using Pandas
* Explored structure using `.info()`, `.describe()`
* Identified missing values and data types

### 2️⃣ Data Cleaning

* Filled missing values:

  * `Age` → Median
  * `Embarked` → Mode
* Dropped `Cabin` due to excessive missing values
* Removed unnecessary columns (`Name`, `Ticket`)

### 3️⃣ Feature Engineering

* Created new feature:

  * `FamilySize = SibSp + Parch + 1`

### 4️⃣ Univariate Analysis

* Distribution of Age, Fare
* Count plots for categorical variables

### 5️⃣ Bivariate Analysis

* Relationship between features and survival:

  * Gender vs Survival
  * Class vs Survival
  * Age vs Survival
  * Fare vs Survival

### 6️⃣ Multivariate Analysis

* Correlation heatmap
* Identified strong and weak relationships

---

## 📈 Key Insights

* ✅ **Gender is the strongest predictor**

  * Females had significantly higher survival rates

* ✅ **Passenger class plays a major role**

  * 1st class passengers had the highest survival probability

* ✅ **Fare is positively correlated with survival**

  * Higher-paying passengers were more likely to survive

* ✅ **Age has a weaker influence**

  * Younger passengers had slightly better chances

* ✅ **Family size impacts survival**

  * Small families had better survival rates than very large or solo travelers

* ❌ **Embarked location has minimal impact**

---

## 🧠 Conclusion

The EDA reveals that survival during the Titanic disaster was strongly influenced by **gender, passenger class, and socio-economic status**.

These insights demonstrate how exploratory data analysis helps uncover hidden patterns and provides a strong foundation for building machine learning models.

---

## ▶️ How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/furqan934/eda-projects.git
   ```

2. Navigate to the project folder:

   ```bash
   cd project_01
   ```

3. Install required libraries:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

---

## 📁 Project Structure

```
titanic-eda-project/
│
├── data/
│   └── train.csv
│
├── notebooks/
│   └── titanic_eda.ipynb
│
├── README.md
└── requirements.txt
```

---

## 🚀 Future Improvements

* Apply machine learning models (Logistic Regression, Random Forest)
* Perform feature scaling and selection
* Build an end-to-end ML pipeline

---

## 👨‍💻 Author

**Muhammad Furqan**

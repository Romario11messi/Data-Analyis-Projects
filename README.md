# 📊 Sales Data Analysis & Data Cleaning Project

## 🚀 Project Overview

This project demonstrates how to perform data cleaning and exploratory
data analysis (EDA) using Python and Pandas.

Dataset: - 250 rows - 10 columns - Multiple null values in numeric and
categorical columns

------------------------------------------------------------------------

## 🔍 Methods Used

### 1️⃣ Detecting Missing Values

``` python
df.info()
df.isnull().sum()
```

### 2️⃣ Dropping Null Values

``` python
df.dropna()
df.dropna(axis=1)
```

### 3️⃣ Filling Null Values

#### Fill with Mean (Recommended for Numeric Data)

``` python
df['Units_Sold'] = df['Units_Sold'].fillna(df['Units_Sold'].mean())
df['Discount_Percent'] = df['Discount_Percent'].fillna(df['Discount_Percent'].mean())
```

#### Replace Invalid Categorical Values

``` python
df['Region'] = df['Region'].replace(0, 'South').fillna('South')
```

------------------------------------------------------------------------

## 🎯 Key Takeaways

-   Data cleaning is essential before analysis.
-   Dropping data can lead to information loss.
-   Numeric and categorical variables require different treatment.
-   Always verify null removal using `df.isnull().sum()`.

------------------------------------------------------------------------

## 🛠 Tools Used

-   Python
-   Pandas
-   Jupyter Notebook

------------------------------------------------------------------------

## 📌 Author

Edward

------------------------------------------------------------------------

This project is part of my data analytics and quantitative portfolio
development.

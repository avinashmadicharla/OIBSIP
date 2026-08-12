# Exploratory Data Analysis on Retail Sales Data

## Oasis Infobyte — Data Analytics Internship

## 1. Project Overview

This project performs Exploratory Data Analysis (EDA) on retail sales transaction data to identify sales patterns, customer demographic trends, product performance, category revenue, relationships between numerical variables, and additional business insights.

The project was completed as part of the Oasis Infobyte Data Analytics Internship under the Data Analytics domain.

---

## 2. Project Objective

The main objective of this project is to transform raw retail sales data into meaningful insights that can support data-driven business decision-making.

The analysis focuses on:

- Understanding the structure and quality of the dataset
- Performing data cleaning and preprocessing
- Calculating descriptive statistics
- Analysing monthly and quarterly sales trends
- Understanding customer age-group and gender distributions
- Identifying the top 10 products by quantity sold
- Analysing revenue by product category
- Studying relationships between numerical variables
- Analysing the relationship between discount levels and profitability
- Providing actionable business recommendations

---

## 3. Dataset

### Dataset Source

The dataset was obtained from Kaggle:

Global Retail Solutions by Patrick Kimunyi.

The Kaggle page lists the dataset license as "Other (specified in description)". The raw dataset is therefore retained locally and is not redistributed through this repository unless the applicable licensing terms are confirmed.

### Dataset Type

Retail sales transaction data.

### Dataset Size

- Records: 200
- Columns: 16

### Available Date Range

January 10, 2024 to July 27, 2024.

### Important Data Fields

The dataset contains information related to:

- Order Date
- Customer demographics
- Product information
- Product category
- Quantity
- Sales Amount
- Discount
- Profit
- Region and other transaction-related attributes

---

## 4. Tools and Technologies

### Programming Language

Python

### Development Environment

Jupyter Notebook

### Python Libraries

- Pandas
- NumPy
- Matplotlib
- Seaborn

---

## 5. Project Structure

```text
DataAnalytics-L1-EDARetailSales/
│
├── data/
│   └── retail sales dataset
│
├── notebooks/
│   └── Retail_Sales_EDA.ipynb
│
├── outputs/
│   ├── monthly_sales.csv
│   ├── quarterly_sales.csv
│   ├── top_10_products.csv
│   ├── category_revenue.csv
│   └── descriptive_statistics.csv
│
├── screenshots/
│   ├── 01_overview.png
│   ├── 02_monthly_sales.png
│   ├── 03_quarterly_sales.png
│   ├── 04_age_groups.png
│   ├── 05_gender_analysis.png
│   ├── 06_top_products.png
│   ├── 07_category_revenue.png
│   ├── 08_correlation_heatmap.png
│   └── 09_discount_profit.png
│
├── README.md
└── requirements.txt
```

---

## 6. Data Preparation

The dataset was inspected to understand its structure, columns, data types, missing values, and duplicate records.

The `Order Date` field was initially stored as a string and was converted into a proper datetime format using Pandas.

This conversion enabled time-based analysis such as monthly and quarterly sales analysis.

The dataset was also checked for missing values and duplicate records.

---

## 7. Exploratory Data Analysis

### 7.1 Descriptive Statistics

Descriptive statistics were calculated to understand the central tendency and variability of numerical variables.

The analysis included:

- Mean
- Median
- Mode
- Standard deviation

---

### 7.2 Monthly Sales Analysis

Monthly sales were calculated by grouping transactions according to the order month.

#### Key Findings

- March 2024 recorded the highest monthly sales with a sales amount of **27,082**.
- January 2024 recorded the lowest monthly sales with a sales amount of **7,533**.

---

### 7.3 Quarterly Sales Analysis

Sales were aggregated by quarter to understand broader sales patterns.

#### Key Finding

Q2 2024 recorded the highest sales among the complete quarters, with a sales amount of **65,960**.

The available data also contains **22,408** in sales for Q3 2024. However, the dataset ends on July 27, 2024, meaning Q3 is only partially represented and should not be directly compared with complete quarters.

---

### 7.4 Customer Age-Group Analysis

Customers were grouped into age categories to understand the distribution of customer records.

#### Key Findings

The largest age group was **26–35**, with **54 records**, followed closely by the **36–45** group with **53 records**.

No records were present for customers under 18 or above 65 in the available dataset.

---

### 7.5 Gender Analysis

Customer records were analysed by gender.

#### Key Finding

The dataset contains an equal distribution of male and female customers:

- Male: 100
- Female: 100

---

### 7.6 Top 10 Products

Products were ranked according to total quantity sold.

#### Top 10 Products

| Rank | Product | Quantity |
|---:|---|---:|
| 1 | Smartphone | 33 |
| 2 | Hat | 33 |
| 3 | Jacket | 32 |
| 4 | Microwave Oven | 31 |
| 5 | Refrigerator | 30 |
| 6 | Gaming Console | 30 |
| 7 | Tablet | 28 |
| 8 | Air Conditioner | 27 |
| 9 | Laptop | 27 |
| 10 | Jeans | 27 |

#### Key Finding

Smartphone and Hat were tied as the highest-volume products, with **33 units sold each**.

---

### 7.7 Revenue by Product Category

Sales were aggregated by product category.

#### Key Finding

**Apparel** generated the highest category revenue, with total sales of **49,467**.

---

### 7.8 Correlation Analysis

A correlation matrix and heatmap were used to examine relationships between numerical variables.

The correlation analysis helps identify variables that move together and can highlight potentially useful relationships for further investigation.

Correlation does not by itself establish causation.

---

### 7.9 Discount and Profitability Analysis

The relationship between discount bands and average profit was analysed.

| Discount Band | Transactions | Average Profit | Total Profit |
|---|---:|---:|---:|
| Low (1–10%) | 44 | 771.20 | 33,932.73 |
| Medium (11–20%) | 83 | 591.55 | 49,098.32 |
| High (21–30%) | 73 | 536.04 | 39,130.92 |

#### Key Finding

An inverse association was observed between discount level and average profit in the available dataset.

Average profit decreased from:

**771.20 → 591.55 → 536.04**

as the discount band increased from Low to Medium to High.

No transactions were recorded in the No Discount and Very High (>30%) categories.

This analysis indicates an observed association and does not establish a causal relationship between discounts and profit.

---

## 8. Overall Sales Performance

The dataset contains total recorded sales of **147,368** across 200 retail transactions.

The available transaction period covers January 10, 2024 to July 27, 2024.

March was the strongest month in terms of sales, while January recorded the lowest monthly sales.

---

## 9. Key Business Insights

The major insights identified from the analysis are:

1. March 2024 was the strongest month based on sales amount.
2. Q2 2024 was the strongest complete quarter in the available dataset.
3. Smartphone and Hat were the highest-volume products.
4. Apparel generated the highest category revenue.
5. Customers aged 26–35 formed the largest age group.
6. Male and female customer records were equally distributed.
7. Higher discount bands were associated with lower average profit in the observed transactions.

---

## 10. Business Recommendations

Based on the analysis, the following recommendations can be considered:

### 1. Focus on High-Performing Products

Maintain sufficient inventory and promotional visibility for products with high sales volume.

### 2. Strengthen High-Revenue Categories

Apparel generated the highest category revenue. The business can continue analysing this category to identify successful products and customer segments.

### 3. Use Customer Demographics

The 26–35 and 36–45 age groups represent the largest observed customer segments. Marketing campaigns can be evaluated against these segments.

### 4. Optimise Discount Strategies

Since higher discount bands were associated with lower average profit, discount strategies should be monitored carefully to balance sales volume and profitability.

### 5. Use Sales Trends for Planning

Monthly and quarterly patterns can support inventory planning, promotional scheduling, and resource allocation.

---

## 11. Project Outcome

The analysis transformed raw retail transaction data into structured statistical and visual insights.

The project demonstrates the use of Python-based exploratory data analysis to examine:

- Sales trends
- Customer demographics
- Product performance
- Category revenue
- Numerical relationships
- Profitability patterns

The resulting insights can support data-driven business decision-making.

---

## 12. How to Run the Project

### Step 1 — Install the required libraries

```bash
pip install -r requirements.txt
```

### Step 2 — Open Jupyter Notebook

```bash
jupyter notebook
```

### Step 3 — Open the project notebook

Navigate to:

```text
notebooks/Retail_Sales_EDA.ipynb
```

### Step 4 — Run the notebook

Run the notebook cells from beginning to end.

---

## 13. Author

**Avinash Madicharla**

Data Analytics Intern

Oasis Infobyte Internship

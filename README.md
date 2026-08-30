📊 Superstore Sales Data Analysis

📌 Project Overview

This project focuses on analyzing a Superstore sales dataset using Python and popular data analysis and visualization libraries.

The analysis explores sales performance, product categories, customer segments, discounts, profits, and delivery time to identify useful business insights.

---

🎯 Objectives

- Analyze Superstore sales data
- Understand sales performance across product categories
- Analyze profit and discount patterns
- Examine customer and regional information
- Calculate delivery time for orders
- Visualize important business insights using charts

---

🛠️ Technologies Used

- Python
- Pandas – Data manipulation and analysis
- NumPy – Numerical operations
- Matplotlib – Data visualization
- Seaborn – Statistical data visualization
- Google Colab / Jupyter Notebook

---

📂 Dataset

The project uses a Superstore sales dataset containing:

- 10,194 records
- 21 original columns

The dataset includes information such as:

- Order ID
- Order Date
- Ship Date
- Ship Mode
- Customer ID
- Customer Name
- Segment
- Country/Region
- City
- State/Province
- Postal Code
- Region
- Product ID
- Category
- Sub-Category
- Product Name
- Sales
- Quantity
- Discount
- Profit

---

🔍 Data Analysis Process

1. Import Libraries

The following Python libraries were used:

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

2. Load Dataset

df = pd.read_csv("samplesuperstore.csv")

3. Data Exploration

The project uses:

- "df.head()"
- "df.info()"
- "df.shape"
- "df.describe()"
- "df.isnull().sum()"

to understand the structure and quality of the dataset.

4. Data Preprocessing

The "Order Date" and "Ship Date" columns were converted into datetime format.

A new column called Delivery Days was created to calculate the number of days taken to deliver each order.

df['Delivery Days'] = (df['Ship Date'] - df['Order Date']).dt.days

---

📈 Analysis Performed

Sales by Category

The project analyzes total sales for the three major product categories:

Category| Total Sales
Technology| 839,893.2790
Furniture| 754,747.7613
Office Supplies| 731,893.3140

Technology has the highest total sales among the three categories.

---

📊 Visualizations

The project includes data visualizations such as:

- Sales by Category
- Category-wise comparisons
- Business performance analysis
- Data distribution and statistical visualizations

Charts are created using Matplotlib and Seaborn.

---

💡 Key Insights

Based on the analysis:

- Technology generates the highest total sales among the categories analyzed.
- Furniture is the second-highest sales category.
- Office Supplies has the lowest total sales among the three major categories.
- The dataset contains both positive and negative profit values, showing that some transactions result in losses.
- Delivery time can be analyzed using the newly created "Delivery Days" feature.
- The dataset contains no missing values in the analyzed columns.

---

📁 Project Structure

Superstore-Sales-Analysis/
│
├── Taskeda1.ipynb
├── samplesuperstore.csv
└── README.md

---

🚀 How to Run the Project

1. Clone the repository

git clone https://github.com/your-username/Superstore-Sales-Analysis.git

2. Open the project

Open "Taskeda1.ipynb" using:

- Google Colab
- Jupyter Notebook
- VS Code

3. Add the dataset

Make sure "samplesuperstore.csv" is available in the correct project location.

4. Run the notebook

Run the cells sequentially to perform the complete analysis.

---

📌 Conclusion

This project demonstrates how Python can be used for data cleaning, exploratory data analysis, business analysis, and data visualization.

The analysis provides an overview of sales performance across different categories and helps identify patterns in sales, profit, discounts, and delivery time.

---

👨‍💻 Author
G.Antro Nithisdon Gowtham 

⭐ If you find this project useful, consider giving the repository a star!
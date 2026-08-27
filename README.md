# 📊 Online Retail Big Data Analysis with PySpark

This project focuses on processing and analyzing the Online Retail dataset using PySpark.

This project was developed as part of a Big Data practical assignment to practice data processing, transformation, and analysis using Apache Spark and PySpark.

## 🎯 Objectives

The main objectives of this project are:

- To learn how to process data using PySpark.
- To work with Spark DataFrames.
- To perform data filtering and transformation.
- To perform grouping and aggregation.
- To apply sorting and repartitioning.
- To perform descriptive statistical analysis.
- To practice basic data cleaning using PySpark.
- To export processed data into CSV format.

## 📊 Dataset

This project uses the **Online Retail dataset** from the UCI Machine Learning Repository.

The dataset contains transaction records from a UK-based online retail business and includes information related to customer purchases and transactions.

The dataset is used as the main source for practicing Big Data processing and analysis using PySpark.

> The raw dataset is not included in this repository.

## 🛠️ Tools & Technologies

- Python
- PySpark
- Apache Spark
- Pandas
- Jupyter Notebook
- Google Colab

## 🔍 Analysis Process

The analysis is performed using PySpark through several data processing stages:

### 1. Spark Session

A Spark Session is created as the entry point for working with Apache Spark.

### 2. Data Loading

The Online Retail dataset is loaded and prepared for processing.

### 3. Data Exploration

The dataset is explored to understand its structure, attributes, and contents.

### 4. PySpark DataFrame

The dataset is converted and processed using a PySpark DataFrame.

### 5. Data Filtering

Filtering operations are performed to select data based on specific conditions.

### 6. Grouping and Aggregation

The `groupBy()` operation is used together with aggregation functions to summarize the data.

### 7. Sorting

The data is sorted based on selected attributes to support further analysis.

### 8. Repartitioning

Repartitioning is performed to practice data partition management in Spark.

### 9. Descriptive Statistics

Descriptive statistical analysis is performed to obtain an overview of the numerical data.

### 10. Data Cleaning

Basic data cleaning operations are performed to prepare the data for analysis.

### 11. Data Export

Processed data is exported into CSV format.

## 📁 Project Structure

```text
online-retail-big-data-analysis/
│
├── README.md
├── requirements.txt
│
└── notebook/
    └── analisis_online_retail.ipynb
##📓 Notebook

The complete implementation and analysis are available in the Jupyter Notebook:

notebook/analisis_online_retail.ipynb

The notebook contains the complete workflow for processing and analyzing the Online Retail dataset using PySpark.

##📚 Learning Outcomes

Through this project, I practiced:

Creating and using a Spark Session.
Working with PySpark DataFrames.
Performing data filtering and transformation.
Using grouping and aggregation operations.
Sorting data using PySpark.
Understanding data repartitioning.
Performing descriptive statistical analysis.
Performing basic data cleaning.
Exporting processed data into CSV format.
🚀 How to Run
1. Clone the repository
git clone https://github.com/USERNAME/online-retail-big-data-analysis.git
cd online-retail-big-data-analysis
2. Install the required libraries
pip install -r requirements.txt
3. Open the notebook

Open:

notebook/analisis_online_retail.ipynb

The notebook can be run using Jupyter Notebook, JupyterLab, or Google Colab.

##📌 Project Context

This project was developed as part of a Big Data practical assignment.

The project focuses on applying fundamental PySpark operations to a real-world retail transaction dataset and gaining practical experience with distributed data processing using Apache Spark.

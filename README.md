# Online Retail Data Analysis with PySpark

An exploratory data analysis project using **Apache PySpark** to process and analyze the **Online Retail Dataset** from the **UCI Machine Learning Repository**.

This project was developed to demonstrate the use of PySpark for processing transactional data, including data exploration, transformation, filtering, aggregation, sorting, partitioning, descriptive statistics, and missing-value handling.

---

## 📌 Project Overview

The **Online Retail Dataset** contains transactional records from a UK-based online retail company.

In this project, the dataset is processed using **Python, Pandas, and Apache PySpark**. The analysis focuses on understanding the structure of the dataset and applying fundamental PySpark DataFrame operations.

The notebook demonstrates how transactional data can be transformed and analyzed using distributed data processing techniques.

---

## 🎯 Objectives

The objectives of this project are:

- Explore the structure and characteristics of the Online Retail dataset.
- Load the dataset and inspect its contents.
- Convert the dataset from Pandas DataFrame to PySpark DataFrame.
- Perform data transformation using PySpark.
- Create a new `TotalPrice` feature.
- Perform filtering based on transaction attributes.
- Perform aggregation using `groupBy()`.
- Sort transaction data based on specific columns.
- Explore Spark partitioning and repartitioning.
- Generate descriptive statistics.
- Identify and handle missing values.
- Export the processed data into CSV format.

---

## 📊 Dataset

This project uses the **Online Retail Dataset** provided by the **UCI Machine Learning Repository**.

### Dataset Source

**UCI Machine Learning Repository — Online Retail**

[View Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

### Dataset Information

| Information | Description |
|---|---|
| Dataset Name | Online Retail |
| Source | UCI Machine Learning Repository |
| Number of Records | 541,909 |
| Time Period | December 2010 – December 2011 |
| File Format | Excel (`.xlsx`) |
| Main Country | United Kingdom |

### Dataset Attributes

| Column | Description |
|---|---|
| `InvoiceNo` | Invoice number of the transaction |
| `StockCode` | Product code |
| `Description` | Product description |
| `Quantity` | Number of products purchased |
| `InvoiceDate` | Date and time of the transaction |
| `UnitPrice` | Price per unit |
| `CustomerID` | Customer identifier |
| `Country` | Customer's country |

---

## 🛠️ Technologies Used

The project uses the following technologies and libraries:

- **Python**
- **Apache PySpark**
- **Pandas**
- **OpenPyXL**
- **Jupyter Notebook**
- **Google Colab**

---

## 🔄 Analysis Workflow

The analysis is performed through several stages.

### 1. Spark Session Initialization

A Spark Session is created as the entry point for working with PySpark.

### 2. Data Loading

The Online Retail dataset is loaded from an Excel file using Pandas.

The Pandas DataFrame is then converted into a **PySpark DataFrame** for further processing.

### 3. Data Exploration

The dataset is explored by examining:

- Dataset dimensions
- Column names
- Data types
- Data schema
- Sample records
- Unique values
- Number of records

### 4. Data Transformation

A new column named `TotalPrice` is created to represent the total value of each transaction.

The calculation is:

`TotalPrice = Quantity × UnitPrice`

This derived feature is then used in subsequent analysis.

### 5. Filtering

Filtering operations are performed to investigate specific subsets of the transactional data.

Examples include:

- Filtering transactions based on `Quantity`.
- Filtering transactions based on `Country`.
- Examining transactions from **France**.

These operations demonstrate the use of PySpark DataFrame filtering.

### 6. Aggregation

Aggregation operations are performed using `groupBy()` to summarize the transactional data.

The analysis includes:

- Aggregating transaction data by country.
- Calculating quantities by product.
- Counting transactions by country.

### 7. Sorting

The data is sorted based on selected attributes, including:

- `TotalPrice`
- `Quantity`

This allows transactions with higher values or quantities to be examined.

### 8. Partitioning and Repartitioning

Spark partitioning is explored to understand how data is distributed across partitions.

The notebook checks the number of existing partitions and demonstrates **repartitioning the DataFrame into four partitions**.

### 9. Descriptive Statistics

Descriptive statistics are generated for numerical variables to provide an overview of the dataset.

This includes measures such as:

- Count
- Mean
- Standard deviation
- Minimum
- Maximum

### 10. Missing Value Handling

The dataset is examined for missing values.

Missing records are then handled using the PySpark `dropna()` operation.

### 11. Data Export

After processing and cleaning, the resulting DataFrame is exported into CSV format for further use.

---

## 📁 Project Structure

```text
online-retail-pyspark/
│
├── notebook/
│   └── online_retail_pyspark_analysis.ipynb
│
├── data/
│   └── README.md
│
├── README.md
├── requirements.txt
└── .gitignore
```

> The original dataset is not included in this repository. Please download the dataset directly from the UCI Machine Learning Repository.

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/USERNAME/online-retail-pyspark.git
cd online-retail-pyspark
```

### 2. Install Dependencies

Install the required Python libraries:

```bash
pip install -r requirements.txt
```

---

## 📥 Dataset Setup

Download the **Online Retail Dataset** from the UCI Machine Learning Repository:

[Download Online Retail Dataset](https://archive.ics.uci.edu/dataset/352/online+retail)

After downloading the dataset, place the Excel file inside the `data/` directory:

```text
data/
└── Online Retail.xlsx
```

Make sure the dataset path used in the notebook matches the location of the downloaded file.

---

## ▶️ How to Run

The notebook can be executed using either **Google Colab**, **Jupyter Notebook**, or **JupyterLab**.

Open the following notebook:

```text
notebook/online_retail_pyspark_analysis.ipynb
```

Then run the cells sequentially from the beginning to the end.

---

## 📈 PySpark Concepts Demonstrated

This project demonstrates several fundamental concepts in PySpark:

| Concept | Implementation |
|---|---|
| Spark Session | `SparkSession` |
| DataFrame Creation | Pandas → PySpark DataFrame |
| Data Exploration | `show()`, `printSchema()`, `count()` |
| Filtering | `filter()` / `where()` |
| Transformation | `withColumn()` |
| Aggregation | `groupBy()` |
| Sorting | `orderBy()` |
| Partitioning | `getNumPartitions()` |
| Repartitioning | `repartition()` |
| Statistics | `describe()` |
| Missing Values | `dropna()` |
| Data Export | `write.csv()` |

---

## 🔍 Analysis Summary

The analysis provides an overview of the transactional dataset and demonstrates how PySpark can be used to process and transform retail transaction data.

Several aspects of the dataset are explored, including:

- Transaction quantities
- Product information
- Transaction prices
- Countries
- Customer information
- Total transaction values
- Missing values
- Spark data partitioning

The notebook primarily focuses on **data processing and exploration using PySpark** rather than predictive modeling or machine learning.

---

## 📚 References

Chen, D. (2015). **Online Retail**. UCI Machine Learning Repository.

- [UCI Machine Learning Repository — Online Retail](https://archive.ics.uci.edu/dataset/352/online+retail)
- [Dataset DOI](https://doi.org/10.24432/C5BW33)

---

## 📄 License

The dataset is provided by the **UCI Machine Learning Repository** under the **CC BY 4.0** license.

For complete information regarding the dataset, licensing, and attribution, please refer to the original dataset source.

---

## 👩‍💻 Author

**Azzahra Anggarista**

This project was created as part of a data processing and analysis project using **Apache PySpark**.

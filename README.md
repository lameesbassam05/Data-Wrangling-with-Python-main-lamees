# Real-World Data Wrangling Project

This project is part of the requirements for the **Palestine Launchpad Program - Data Analysis NanoDegree**. It demonstrates skills in data gathering, quality assessment, cleaning, and transforming data from various sources into a single, analysis-ready dataset.

## 📝 Project Description

This project aims to analyze traffic on an e-commerce website over a five-year period (2019–2023). It covers the entire data wrangling process, starting with data collection from multiple sources (CSV files and databases) and proceeding to cleaning and consolidation for exploratory analysis.

### ✨ Skills Demonstrated:

- **Gathering Data:** Extracting data from CSV files and SQL databases.
- **Assessing Data:** Identifying quality issues and structural (tidiness) issues.
- **Cleaning Data:** Addressing identified issues such as outliers and incorrect data types, as well as merging tables.
- **Exploratory Data Analysis (EDA):** Using visualizations to understand patterns and trends in user behavior and website traffic.

## 📊 Data Sources

Data was collected from two different sources:

1.  **`download.csv`**: A CSV file containing daily website traffic data from **2019 to 2021**.
2.  **`eco.sql`**: A MySQL database file containing daily traffic data for the years **2022 and 2023**. Python was used to connect to the database, extract this data, and save it to a file named `extracted_data.csv`. ## 🛠️ Tools and Technologies

- **Language:** Python 3
- **Libraries:**
- `Pandas`: For data loading, cleaning, merging, and analysis. 
- `NumPy`: For numerical operations. 
- `Matplotlib` & `Seaborn`: For creating charts and visualizations. 
- `pymysql`: For connecting to the MySQL database and extracting data.
- **Databases:** MySQL

## 🧹 Key Data Cleaning Process

Several data quality and structural issues were addressed, including:

- **Date Format Standardization:** Converted all dates from various formats (e.g., `MM/DD/YYYY`) to a unified format (`YYYY-MM-DD`).
- **Handling Outliers:** Identified outliers in numerical columns using the Interquartile Range (IQR) method and excluded them to ensure more accurate analysis.
- **Data Merging:** Combined the dataset from the CSV file with the dataset extracted from the database to create a comprehensive dataset (`cleaned_ecommerce_data.csv`) covering the period from 2019 to 2023.
- **Data Structure Optimization (Tidiness):** Separated improperly combined columns—such as the "Visitors" column—to ensure each column represents a single variable.

## 📈 Summary of Key Findings

- **Traffic Distribution:** Analyzing traffic distribution over the years reveals peak periods and lulls in user engagement.
- **Session Duration:** Analyzing average session duration provides insights into the level of user engagement with the website's content. - **Annual patterns:** The data reveals clear seasonal fluctuations in traffic, which can assist in planning future marketing campaigns.

## 🚀 How to Use

1.  **Clone the repository:**
```bash
git clone https://github.com/YOUR-USERNAME/Data-Wrangling-with-Python.git

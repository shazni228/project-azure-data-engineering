# Tokyo Olympic Azure Data Engineering Project

## Project Overview

This project demonstrates an end-to-end Azure Data Engineering pipeline using Tokyo Olympic datasets. The objective is to ingest raw Olympic data, transform it using Azure cloud services, store it in a structured format, and perform analytical queries to generate insights.

The project showcases practical implementation of modern data engineering concepts including data ingestion, transformation, storage, orchestration, and analytics using Microsoft Azure services.

## Architecture

The project follows a modern data engineering architecture:

1. Data Source (CSV Files)
2. Azure Data Lake Storage Gen2
3. Azure Data Factory for data ingestion
4. Azure Databricks for data transformation
5. Azure Synapse Analytics for querying and reporting
6. Visualization and analysis of Olympic data

### Data Flow

CSV Files → Azure Data Factory → Azure Data Lake Storage → Azure Databricks → Azure Synapse Analytics → Reporting & Insights

---

## Dataset Description

The project uses Tokyo Olympic datasets containing information about athletes, coaches, teams, medals, and gender participation.

### Files Included

#### Athletes.csv

Contains athlete information including:

* Athlete Name
* Country
* Discipline

#### Coaches.csv

Contains coach information including:

* Coach Name
* Country
* Discipline

#### Teams.csv

Contains team participation details including:

* Team Name
* Country
* Event

#### Medals.csv

Contains medal statistics including:

* Country
* Gold Medals
* Silver Medals
* Bronze Medals
* Total Medals

#### EntriesGender.csv

Contains gender participation statistics including:

* Discipline
* Female Participants
* Male Participants
* Total Participants

---

## Azure Services Used

### Azure Data Factory (ADF)

Used to:

* Ingest raw CSV files
* Create automated data pipelines
* Move data into Azure Data Lake Storage

### Azure Data Lake Storage Gen2 (ADLS)

Used as:

* Centralized storage layer
* Repository for raw and transformed datasets
* Scalable cloud-based data lake

### Azure Databricks

Used for:

* Data cleansing
* Data transformation
* Data validation
* Feature engineering
* Data aggregation

### Azure Synapse Analytics

Used for:

* Querying transformed datasets
* Performing analytical operations
* Generating business insights

---

## Project Structure

```text
tokyo-olympic-azure-data-engineering-project/
│
├── data/
│   ├── Athletes.csv
│   ├── Coaches.csv
│   ├── EntriesGender.csv
│   ├── Medals.csv
│   └── Teams.csv
│
├── transformation/
│   ├── data_transformation.py
│   └── notebooks/
│
├── screenshots/
│   ├── adf_pipeline.png
│   ├── databricks_transformation.png
│   └── synapse_query_results.png
│
├── README.md
└── requirements.txt
```

---

## Data Engineering Workflow

### Step 1: Data Ingestion

* Upload Olympic CSV files to Azure Data Lake Storage.
* Configure Azure Data Factory pipelines.
* Automate data movement from source to storage.

### Step 2: Data Transformation

Using Azure Databricks:

* Read raw CSV files.
* Handle missing values.
* Standardize column names.
* Convert data types.
* Aggregate medal counts.
* Generate analytical datasets.

### Step 3: Data Storage

Store transformed datasets in:

* Azure Data Lake Storage
* Parquet format for optimized performance

### Step 4: Analytics

Analyze:

* Country-wise medal distribution
* Gender participation trends
* Team performance
* Athlete participation by discipline
* Coach distribution across sports

---

## Sample Analysis Performed

### Top Countries by Total Medals

Identify countries with the highest medal counts.

### Gender Participation Analysis

Compare male and female athlete participation across sports disciplines.

### Discipline-wise Athlete Distribution

Analyze athlete representation across different Olympic sports.

### Coach Participation Analysis

Evaluate coaching representation by country and discipline.

---

## Technologies Used

* Microsoft Azure
* Azure Data Factory
* Azure Data Lake Storage Gen2
* Azure Databricks
* Azure Synapse Analytics
* Apache Spark
* PySpark
* Python
* SQL

---

## Key Learnings

* Building cloud-native ETL pipelines
* Working with Azure Data Factory orchestration
* Managing large datasets in Azure Data Lake
* Transforming data using PySpark
* Performing analytics using Azure Synapse
* Implementing modern data engineering best practices

---

## Future Enhancements

* Real-time Olympic data streaming
* Power BI dashboard integration
* Incremental data loading
* CI/CD pipeline implementation
* Automated monitoring and alerting
* Data quality validation framework

---

## Getting Started

### Prerequisites

* Azure Subscription
* Azure Data Factory
* Azure Data Lake Storage Gen2
* Azure Databricks Workspace
* Azure Synapse Analytics Workspace

### Setup

1. Clone the repository.

```bash
git clone https://github.com/your-username/tokyo-olympic-azure-data-engineering-project.git
```

2. Upload the CSV files to Azure Data Lake Storage.

3. Configure Azure Data Factory pipelines.

4. Execute Databricks notebooks for transformation.

5. Query transformed datasets using Azure Synapse Analytics.

---

## Results

The project successfully demonstrates an end-to-end Azure Data Engineering solution capable of ingesting, transforming, storing, and analyzing Olympic datasets using scalable cloud-native technologies.

---

## Author

**Shazni Ahamed**

Data Analytics | Business Intelligence | Data Engineering

Website: https://shazni.web.app

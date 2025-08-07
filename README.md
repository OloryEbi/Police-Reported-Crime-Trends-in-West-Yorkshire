# 📊 Police-Reported Crime Trends Analysis (West Yorkshire, Apr–Sep 2020)

This repository contains a comprehensive data analysis pipeline developed for the **Data Scientist Development Programme (DSDP)** interview at the **Leeds Institute for Data Analytics (LIDA)**. It explores police-reported street-level crime trends in West Yorkshire between April and September 2020.

---

## 🎯 Objectives

* Analyse monthly trends and variations in crime counts.
* Identify patterns and anomalies across crime types.
* Highlight potential data quality issues and recommend further analytical steps.

![WhatsApp Image 2025-08-07 at 03 39 22_940455ec](https://github.com/user-attachments/assets/21704fd7-da70-4749-a13e-e0905181db88)

---

## 📚 Project Overview

Street-level crime data provides valuable insights for law enforcement, local government and policymakers. This analysis involved detailed data exploration, cleaning, visualisation and interpretation to reveal actionable insights from six months of crime records.

### 🛠️ Key Analytical Steps

#### 1️⃣ Data Collection and Loading

* Programmatically loaded and combined monthly crime data from CSV files for scalable and reproducible analysis.

#### 2️⃣ Data Cleaning and Preprocessing

* Removed irrelevant columns (e.g., empty or constant-value columns).
* Dropped records missing essential fields (e.g., Crime type).
* Filtered out unrealistic geographic coordinates outside West Yorkshire boundaries.
* Removed duplicate records to prevent data inflation.
* Standardised textual data for crime types and outcome categories.
* Converted months into ordered categorical data for accurate temporal analysis.
* Validated and corrected inconsistencies in location (LSOA) naming conventions.

#### 3️⃣ Exploratory Data Analysis (EDA)

* Initial exploration identified missing data, outliers and key data quality concerns.
* Monthly and categorical breakdown of crime data to identify trends.

#### 4️⃣ Data Visualisation

* Created clear, informative visuals including:

  * Line charts for monthly crime trends.
  * Stacked bar charts for crime type distribution.
  * KDE heatmaps for spatial crime density analysis.
  * Comparative bar charts for month-to-month crime changes.

#### 5️⃣ Anomaly and Quality Detection

* Investigated anomalies, especially missing Crime IDs.
* Highlighted inconsistencies such as ambiguous or repeated location labels.

---

## 📌 Key Findings

### Monthly Crime Trends

* Crime counts gradually rose from April, peaked in August and slightly decreased in September, aligning with easing COVID-19 restrictions and seasonal patterns.  

### Crime Type Distribution

* Most frequent crime types were:

  * **Violence and Sexual Offences**
  * **Anti-Social Behaviour**
  * **Public Order Offences**

### Crime Hotspots (LSOAs)

* Highest crime densities observed in densely populated urban areas, notably Leeds and Bradford, indicating a potential focus for targeted interventions.  

### Spatial Crime Density

* KDE heatmap highlighted high-density crime clusters in urban centres like Leeds, Bradford, Wakefield, Huddersfield and Halifax.

---

## ⚙️ Tools and Technologies

* **Languages:** Python

   **Libraries:**

  * pandas
  * numpy
  * matplotlib
  * seaborn

* **Environment:**

  * Jupyter Notebook

---

## 🚧 Data Quality Observations

* Approximately 14% of records lacked unique Crime IDs, notably affecting "Anti-Social Behaviour" cases.
* Vague or repetitive location labels (e.g., "No Location") reduced spatial precision.
* Lack of detailed timestamps limited finer-grained temporal analyses.

---

## 🚀 Recommendations for Further Analysis

### Immediate Steps:

* Conduct detailed monthly analyses by crime type.
* Analyse crime outcomes and resolution efficiency by location and type.
* Further refine data quality checks and address missing or ambiguous entries.

### Long-Term Goals:

* Create interactive crime mapping tools for real-time analysis.
* Develop predictive models to forecast future crime hotspots.
* Engage with data providers to enhance the quality and completeness of collected data.

---

## 📥 Data Access

Due to file size and licensing restrictions, raw data files are not included. Please access data from:

* 🔗 [Official Source (data.police.uk)](https://data.police.uk/data/)
* 🔗 [DSDP Task Data Link](https://tinyurl.com/DSDP25)

Follow instructions in [`data/README.txt`](data/README.txt) to structure data for analysis.

---

## 💻 How to Run

### Environment Setup

```bash
pip install -r requirements.txt
```

### Analysis Execution

1. Open `crime_analysis.ipynb` using Jupyter Notebook.
2. Execute notebook cells sequentially from data loading through visualisation outputs.

---

## 🙌 Acknowledgements

* Leeds Institute for Data Analytics (LIDA)
* University of Leeds (Visit the official [University of Leeds website](https://www.leeds.ac.uk)   
* UK Police Data Platform ([data.police.uk](https://data.police.uk))

🙏 Special thanks to the data science and open-source communities.


---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---


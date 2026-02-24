# PharmaGuard
*A data engineering pipeline for drug information collection, processing, and visualization*

**Author:** Ninh Giang Nguyen

---

## 🛠 Skills & Technologies

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-D71F00?style=for-the-badge&logo=sqlalchemy&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-59666C?style=for-the-badge&logoColor=white)
![OpenFDA](https://img.shields.io/badge/OpenFDA%20API-0071BC?style=for-the-badge&logoColor=white)
![DailyMed](https://img.shields.io/badge/DailyMed%20API-00897B?style=for-the-badge&logoColor=white)
![MedlinePlus](https://img.shields.io/badge/MedlinePlus%20API-007A5E?style=for-the-badge&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=for-the-badge&logoColor=white)
![WordCloud](https://img.shields.io/badge/WordCloud-E91E63?style=for-the-badge&logoColor=white)

---

## Overview

**PharmaGuard** is a comprehensive data engineering system designed to collect, process, and visualize drug information from public health APIs and web sources. It bridges the gap between **data engineering and health data science**, with potential applications for pharmacists, healthcare providers, and consumers seeking to manage medications safely.

---

## Key Features

###  Data Collection
- Fetches drug data from **OpenFDA**, **DailyMed**, and **MedlinePlus** APIs
- Supplements API data with **web scraping** via BeautifulSoup

###  Data Preprocessing
- Cleans and normalizes data — handles missing values, standardizes text fields, and removes duplicates
- Stores structured data in a **MySQL relational database** across three tables:

| Table | Description |
|---|---|
| Drug Details | Core drug information and attributes |
| Recall Tracking | Historical and active drug recall records |
| Adverse Event Notifications | Reported side effects and safety signals |

### Visualization
- Word clouds, pie charts, and distribution plots to surface patterns in the data
- Interactive outputs via **Plotly** for exploratory analysis
<img width="651" alt="image" src="https://github.com/user-attachments/assets/4294f617-59f3-4f37-bbb6-90a38b6fbe95" />

---

##  Quick Start

### Prerequisites
- Python 3.x
- MySQL
- Virtual environment (venv or Pipenv)
- API credentials (if required for OpenFDA / DailyMed)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/ninhgiangnguyen/Drug_data_engineering_project.git
   cd Drug_data_engineering_project
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python3 -m venv env
   source env/bin/activate      # Linux / macOS
   env\Scripts\activate         # Windows
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the pipeline:**
   ```bash
   python data_collection.py       # Fetch drug data from APIs & web scraping
   python data_preprocessing.py    # Clean, normalize, and store to MySQL
   ```

---

## Challenges & Future Improvements

**Current Limitations:**
- Access to detailed drug data is restricted due to its sensitive nature, limiting opportunities for model training or predictive analytics.
- The project currently focuses on the data engineering layer — extraction, storage, and cleaning — rather than downstream modeling.

**Planned Improvements:**
- Secure access to licensed datasets for richer insights and model training
- Develop predictive models for adverse event detection once data constraints are resolved
- Explore additional data sources and optimize the collection pipeline

---

*Built to bridge the gap between data engineering and healthcare analytics.*


   

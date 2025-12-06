# Netflix-Movies-TV-Shows-Data-Analysis
# 📺 Netflix Movies & TV Shows Data Analysis  
**Python • Power BI • Data Cleaning • Data Visualization**

This project explores and analyzes the Netflix global catalog of Movies and TV Shows using **Python for data preprocessing** and **Power BI for interactive visualization**.

The workflow includes:
- Cleaning and transforming the raw dataset  
- Feature engineering (e.g., extracting year added & exploding genres)  
- Building a relational data model in Power BI  
- Creating interactive visuals and insights about Netflix content  

---

## 🚀 Project Overview

The goal of the project is to uncover meaningful insights about Netflix content, such as:

- Movies vs TV Shows distribution  
- Most common genres  
- Top-producing countries  
- Trends in content additions over the years  
- Metadata patterns such as directors, release years, and categories  

The final output is a **fully interactive Power BI dashboard** supported by a **cleaned and transformed dataset** created in Python.

---

## 📂 Dataset Description

The dataset contains information about Netflix Movies and TV Shows, including:

| Column | Description |
|--------|-------------|
| `show_id` | Unique content identifier |
| `type` | Movie or TV Show |
| `title` | Title of the content |
| `director` | Director name |
| `cast` | List of actors |
| `country` | Producing countries |
| `date_added` | Date content was added to Netflix |
| `release_year` | Year content was originally released |
| `rating` | Age rating |
| `duration` | Runtime or number of seasons |
| `listed_in` | Genres/categories |
| `description` | Summary overview |

---

## 🧰 Tools & Technologies

### **Python (JupyterLite)**
- Pandas (cleaning, transformations)
- NumPy
- Matplotlib (basic plots)

### **Power BI**
- Data modeling (relationships via show_id)
- Visual analytics
- DAX measures
- Interactive filters & slicers

---

## 🔄 Workflow Summary

### **1. Data Cleaning in Python**
Performed inside JupyterLite:

- Loaded raw `my_netflix_dataset.csv`
- Cleaned missing values in:
  - `director`, `cast`, `country`, `duration`, `rating`
- Parsed dates using:
  ```python
  df['date_added'] = pd.to_datetime(df['date_added'], errors='coerce')

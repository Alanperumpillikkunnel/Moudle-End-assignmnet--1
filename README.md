# Moudle-End-assignmnet--1  
# Healthcare Data Analysis & Interactive Dashboard

A comprehensive multi-part healthcare data analysis project built using **Excel/Google Sheets**. This project involves data cleaning, structural integration, advanced exploratory data analysis (EDA), statistical modeling, and an interactive dashboard featuring dynamic slicers.

---

## 📋 Project Overview & Objectives
The goal of this assignment is to process and integrate fractured healthcare records into a unified master dataset, explore correlations between clinical metrics, and build an interactive reporting dashboard to analyze patient outcomes based on lifestyle, demographics, and medical history.

* **Datasets Integrated**: Medical Examinations, Hospitalization Details, and Customer Names.
* **Primary Key**: `Customer ID`
* **Analysis Scope**: 
  * Patient demographics (Age calculation, Date formatting).
  * Medical history correlations (Cancer history vs. Smoking status, Transplants vs. Surgeries/HbA1C).
  * Cost analysis (Charges across Weight Status, Diabetes Status, and Regional Hospital Tiers).
  * Correlation tracking (Age vs. BMI, HbA1C, and Healthcare Charges).

---

## 🛠️ Technical Tools & Functions Used
* **Data Integration & Lookup**: `VLOOKUP`, `XLOOKUP`
* **Date & Math Logic**: `DATE`, `DATEDIF`, `YEARFRAC`, `INT`, `COLUMN()`
* **Data Aggregation**: Pivot Tables & Pivot Charts
* **Interactivity**: Connected Slicers (`Weight Status`, `Diabetes Status`)

---

## 📂 Project Structure & Methodology

1. **Data Cleaning & Preprocessing**:
   * Standardized text and boolean inconsistencies (e.g., `smoker`, `Heart Issues`, `NumberOfMajorSurgeries`).
   * Consolidated separate Year, Month, and Day columns into a uniform **`Date of Birth`** field.
   * Computed exact **`Age`** as of the dataset collection date (**June 8, 2023**).
   * Formatted monetary metrics as currency (`$`).

2. **Master Sheet Integration (`Healthcare`)**:
   * Merged the three source tables into a single cohesive sheet using `Customer ID` as the relational anchor.
   * Retained mandatory schema: *Customer ID, First Name, BMI, HBA1C, Heart Issues, Any Transplants, Cancer history, NumberOfMajorSurgeries, smoker, Weight Status, Diabetes Status, Date of Birth, charges, Hospital tier, City tier, State ID, Age.*

3. **Exploratory Data Analysis & Visualizations**:
   * **Pie / Donut Charts**: Evaluated cancer history distribution among smokers vs. non-smokers.
   * **Column / Bar Charts**: Compared major surgeries and HbA1C variations based on transplant history, alongside cost distributions across weight and diabetes classifications.
   * **Scatter Plots & Trendlines**: Explored linear relationships and correlations between age, BMI, HbA1C, and healthcare charges.

4. **Interactive Dashboard**:
   * Centralized all visual components onto a single unified canvas.
   * Integrated synchronized **Slicers** for `Weight Status` and `Diabetes Status` connected across all underlying pivot tables for real-time cross-filtering.

---

## 🚀 How to View / Run
1. Download the `.xlsx` file from this repository.
2. Open it in **Microsoft Excel** or upload it to **Google Sheets**.
3. Ensure macro or data connections are enabled if prompted to allow the slicers and pivot tables to function interactively.

---
*Author: [Your Name]*

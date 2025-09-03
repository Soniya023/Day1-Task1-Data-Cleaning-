# Task 1: Data Cleaning and Preprocessing

## Overview
This project focuses on cleaning and preparing the **Medical Appointment No Shows** dataset for analysis. The dataset had issues like inconsistent column names, missing or incorrect values, and unstandardized categorical data. Using **Python (Pandas)**, all necessary preprocessing steps were applied to make the dataset analysis-ready.

## Dataset
- **Source:** Kaggle – [Medical Appointment No Shows](https://www.kaggle.com/joniarroba/noshowappointments)  
- **Rows:** 110,527  
- **Columns:** 14  
- **Key Features:**  
  - PatientID, AppointmentID  
  - Gender, Age, Neighbourhood  
  - ScheduledDay, AppointmentDay  
  - Scholarship, Hypertension, Diabetes, Alcoholism, Handicap, SMS_received  
  - No-show  

## Cleaning Steps
1. **Column Standardization:** Renamed all columns to lowercase and replaced spaces with underscores. Fixed typos (`hipertension` → `hypertension`, `handcap` → `handicap`).  
2. **Date Conversion:** Converted `scheduledday` and `appointmentday` to datetime format.  
3. **Age Cleaning:** Removed negative and unrealistic age values; verified statistics (min, max, mean).  
4. **Duplicate Removal:** Checked for duplicates; none found.  
5. **Gender Standardization:** Replaced `F/M` with `Female/Male`.  
6. **No-show Column:** Clarified labels as `Showed Up` and `No Show`.  
7. **Binary Columns Verification:** Ensured binary columns (`Scholarship`, `Hypertension`, `Diabetes`, `Alcoholism`, `Handicap`, `SMS_received`) were correctly encoded as 0/1.  
8. **Neighbourhood Cleaning:** Converted to lowercase, removed accents and extra spaces.  
9. **Verification:** Checked missing values, data types, and sample data to ensure dataset is clean and analysis-ready.  

## Deliverables
- `cleaned_medical_appointments.csv` – Cleaned dataset  
- `data_cleaning.ipynb` – Python code for cleaning  
- `screenshots/` – Optional verification screenshots  

## Outcome
The cleaned dataset is ready for:  
- Patient no-show prediction  
- Neighborhood-based attendance trends  
- Health condition analysis (Diabetes, Hypertension, etc.)  
- Visualization of age, gender, and appointment patterns  

## Note
All preprocessing steps were carefully documented and verified to ensure **reliability** and **reproducibility**, allowing confident use for further analysis or modeling.

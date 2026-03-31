# 🩺 Blood Pressure Data Engineering Project

## 📌 Deskripsi Project
Project ini merupakan implementasi sederhana dari proses Data Engineering menggunakan dataset tekanan darah global. Dataset ini mengacu pada data kesehatan yang relevan dengan laporan World Health Organization (WHO) mengenai prevalensi hipertensi di dunia.

Tujuan dari project ini adalah untuk melakukan proses end-to-end data pipeline mulai dari pengambilan data mentah hingga menghasilkan data yang siap digunakan.

---

## 📊 Dataset
- Sumber: Kaggle
- Topik: Global Blood Pressure & Hypertension
- Format: CSV

Dataset berisi informasi seperti:
- Country
- Year
- Systolic & Diastolic Blood Pressure
- BMI
- Smoking Status
- Hypertension Status

---

## ⚙️ Proses Data Engineering

### 1. Data Collection
Dataset diambil dari Kaggle dalam format CSV sebagai raw data.

### 2. Data Cleaning & Data Quality Check
- Menghapus missing values (dropna)
- Menghapus data duplikat (drop_duplicates)
- Normalisasi nama kolom
- Validasi tipe data

### 3. Data Filtering
Kolom yang digunakan:
- country
- year
- systolic_bp_mmhg
- diastolic_bp_mmhg
- bmi
- smoking_status
- bp_category

### 4. Data Transformation
Menambahkan kategori tekanan darah berdasarkan nilai systolic.

### 5. Data Export
- Excel: cleaned_blood_pressure.xlsx
- SQL: blood_pressure_clean.sql

---

## 🛡️ Data Governance

### Data Dictionary
File: data_dictionary.xlsx

### Data Masking
Dataset tidak mengandung data sensitif, sehingga masking tidak diperlukan.

---

## 🛠️ Tools
- Python
- Pandas
- Jupyter Notebook

---

## 📁 Struktur Project
- blood_pressure_global_dataset.csv
- data_engineering_bp.ipynb
- cleaned_blood_pressure.xlsx
- blood_pressure_clean.sql
- data_dictionary.xlsx
- README.md

---

## 🚀 Cara Menjalankan
1. Install library:
pip install pandas openpyxl

2. Jalankan notebook:
data_engineering_bp.ipynb

---

## 🎯 Kesimpulan
Project ini mencakup proses dasar data engineering:
- Data cleaning
- Data transformation
- Data governance
- Data export


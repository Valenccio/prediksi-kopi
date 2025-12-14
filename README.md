# Coffee Sales Prediction Dashboard

A simple **machine learning web app** built with **Python and Streamlit** to predict daily coffee sales based on:
- coffee type
- customer gender
- customer age
- order time (hour of the day)

This project is part of my personal portfolio to demonstrate my understanding of the **software development process** (from data preparation, model training, to deployment on the web).

---

## Features

### 1. Coffee Sales Prediction
- Input:
  - Coffee type (Americano, Latte, Cappuccino, Mocha, Espresso)
  - Customer gender (Male / Female)
  - Age
  - Hour of order (0–23)
- Output:
  - Predicted number of cups sold at that specific hour.
- Optional:
  - Compare **two coffee types** side-by-side at the same time.

### 2. Hourly Prediction Chart (0–23)
- Generates a **line chart** of predicted coffee sales for every hour (0–23).
- Can show:
  - Only one coffee type, or
  - Two coffee types on the same chart for comparison.

### 3. Data Exploration Page
- Interactive filters in the sidebar:
  - Coffee type
  - Customer gender
  - Hour range
- Visualizations:
  - Total sales per coffee type
  - Average cups per hour
  - Average sales by coffee type and gender
- Shows basic statistics:
  - Total rows
  - Average cups sold
  - Average customer age

### 4. Multi-page Streamlit App
- `Home` page → project introduction and usage guide
- `Prediksi Kopi` page → main prediction interface
- `Eksplorasi Data` page → data analytics and visualizations

---

## Tech Stack / Technologies Used

- **Language:** Python
- **Web Framework:** [Streamlit](https://streamlit.io/)
- **Machine Learning:**
  - scikit-learn (RandomForestRegressor)
- **Data Handling:** pandas, numpy
- **Model Persistence:** joblib
- **Visualization:** Streamlit built-in charts (line chart, bar chart)
- **Version Control & Hosting:** Git, GitHub, Streamlit Community Cloud

---

Link deployed for demo: https://prediksi-kopi-x3uem39z4al9n8vkrmuwz9.streamlit.app/prediksi_kopi

---

##  Project Structure

```text
.
├─ home.py                  
├─ requirements.txt
├─ README.md
├─ data/
│  └─ data_kopi.csv       
├─ models/
│  └─ model_kopi.pkl        
├─ assets/
│  ├─ bg.jpg                
└─ pages/
   ├─ 1_Prediksi_Kopi.py    
   └─ 2_Eksplorasi_Data.py  

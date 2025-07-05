# 🔥 Algerian Forest Fire Risk Prediction Web App

This is a Flask-based machine learning web application that predicts the risk of **forest fires in Algeria** using environmental data. It uses a trained **Ridge Regression** model and the **Algerian Forest Fires Dataset** collected between June and September 2012.

---

## 🌍 Dataset Description

The dataset includes **244 observations** from two Algerian regions:

- **Bejaia (Northeast Algeria)** – 122 samples  
- **Sidi Bel-Abbes (Northwest Algeria)** – 122 samples  

Each instance contains meteorological data and fire weather indexes, observed between **June to September 2012**. The data is labeled as either **Fire** or **Not Fire**.

### 📊 Attributes:

| Feature | Description |
|--------|-------------|
| 1. Date        | Observation Date (DD/MM/YYYY) |
| 2. Temp        | Temperature at noon (°C) — range: 22 to 42 |
| 3. RH          | Relative Humidity (%) — range: 21 to 90 |
| 4. Ws          | Wind Speed (km/h) — range: 6 to 29 |
| 5. Rain        | Daily Rainfall (mm) — range: 0 to 16.8 |
| 6. FFMC        | Fine Fuel Moisture Code — range: 28.6 to 92.5 |
| 7. DMC         | Duff Moisture Code — range: 1.1 to 65.9 |
| 8. DC          | Drought Code — range: 7 to 220.4 *(Not used in model)* |
| 9. ISI         | Initial Spread Index — range: 0 to 18.5 |
| 10. BUI        | Buildup Index — range: 1.1 to 68 *(Not used in model)* |
| 11. FWI        | Fire Weather Index — range: 0 to 31.1 *(May be used as target)* |
| 12. Classes    | **Output Label**: Fire / Not Fire |

---

## 🤖 Project Overview

This project demonstrates the deployment of a **machine learning model** via a **Flask web interface**. The user can input weather and fire index values, and the model will predict the likelihood or severity of a forest fire based on training from the Algerian dataset.

---

## 🧠 Machine Learning Model

- **Model**: Ridge Regression
- **Scaler**: StandardScaler
- **Target**: Fire Weather Index (FWI) or Binary Fire Class (depending on version)
- **Features Used**: Temp, RH, Ws, Rain, FFMC, DMC, ISI, Classes (converted), Region

---

## 🖥️ Web App Features

- Clean UI built using HTML and Flask
- Takes 9 input features from the user
- Scales input with `StandardScaler`
- Predicts output using a pickled Ridge Regression model
- Displays prediction result on a result page

---

## 📁 Project Structure





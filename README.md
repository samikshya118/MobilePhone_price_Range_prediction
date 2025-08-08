# 📱 Mobile Price Range Prediction

## 📌 Objective
The aim of this project is to explore and analyze mobile phone specifications data and build a machine learning system that can classify mobile phones into different **price ranges** based on their features.  

The price range categories are:  
- **0 → Low Cost**  
- **1 → Medium Cost**  
- **2 → High Cost**  
- **3 → Very High Cost**  

Currently, the project is in the **Exploratory Data Analysis (EDA)** and **initial model training** stage.

---

## 📊 Dataset
The dataset contains information about various mobile phones, their specifications, and their price category.

### **Features**
| Column        | Description |
|---------------|-------------|
| `battery_power` | Battery capacity in mAh |
| `blue` | Has Bluetooth (1 = Yes, 0 = No) |
| `clock_speed` | Processor speed (in GHz) |
| `dual_sim` | Dual SIM support (1 = Yes, 0 = No) |
| `fc` | Front camera megapixels |
| `four_g` | Has 4G (1 = Yes, 0 = No) |
| `int_memory` | Internal memory in GB |
| `m_dep` | Mobile depth in cm |
| `mobile_wt` | Weight of mobile phone in grams |
| `n_cores` | Number of processor cores |
| `pc` | Primary camera megapixels |
| `px_height` | Pixel resolution height |
| `px_width` | Pixel resolution width |
| `ram` | RAM in MB |
| `sc_h` | Screen height in cm |
| `sc_w` | Screen width in cm |
| `talk_time` | Battery life in hours (single charge) |
| `three_g` | Has 3G (1 = Yes, 0 = No) |
| `touch_screen` | Has touch screen (1 = Yes, 0 = No) |
| `wifi` | Has WiFi (1 = Yes, 0 = No) |
| `price_range` | **Target Variable**: 0 = Low, 1 = Medium, 2 = High, 3 = Very High |

---

## 🛠️ Current Progress
1. **Exploratory Data Analysis (EDA)**
   - Checked for missing values and data types.
   - Analyzed feature distributions and relationships with `price_range`.
   - Visualized correlations using heatmaps and scatterplots.
2. **Preprocessing**
   - No missing values detected.
   - All categorical values already in numeric format (binary flags).
3. **Initial Modeling**
   - Implemented and evaluated:
     - **Logistic Regression**
     - **Random Forest Classifier**
4. **Results**
   | Model                  | Accuracy Score |
   |------------------------|----------------|
   | Logistic Regression    | **0.90**       |
   | Random Forest Classifier | 0.88        |
   > Logistic Regression outperformed Random Forest in this dataset.
5. **Observations**
   - Features like **RAM**, **Pixel Resolution**, and **Battery Power** showed strong influence on price range.


---

## 🚀 Tech Stack
- **Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Environment:** Jupyter Notebook / Google Colab

---

# 📊 COVID-19 Data Analysis and Visualization

This project performs data cleaning, analysis, and visualization of a COVID-19 dataset. It highlights trends in case rates, hospitalization rates, death rates, age-wise hospitalization, race-wise comparisons, and correlation over time.

---

## 📁 Dataset

The dataset used is assumed to be a CSV file named `python.csv` located in the `/content/` directory. It should include COVID-19 statistics such as:

- Date
- Cases and hospitalization rates
- Death rates
- Age-specific hospitalization data
- Race-specific cases and hospitalizations

---

## 🔧 Data Cleaning Steps

The initial preprocessing includes:

- Removing duplicate records
- Dropping columns with over 40% missing values
- Filling missing numeric values with the column median
- Filling missing categorical values with the mode
- Converting the date column to proper datetime format
- Lowercasing and trimming string values
- Removing outliers using Z-score (keeping data within 3 standard deviations)

---

## 📈 Visualizations

### 1. 📉 **Line Chart: Hospitalization vs Death Rate Over Time**

- **Metrics:** `Hospitalizations Rate - Total` vs `Deaths Rate - Total`
- Displays trend comparison over time using a line plot.

### 2. 👶👵 **Bar Chart: Age-Wise Average Hospitalization Rate**

- Shows average hospitalization rate across age groups:
  - Age 0-17 to 80+

### 3. 🧑🏽‍🦱🧑🏻‍🦳 **Bar Chart: Race-Wise Case vs Hospitalization Rate**

- Compares:
  - `Cases - Latinx`, `Cases - Black Non-Latinx`, etc.
  - `Hospitalizations` for the same race groups

### 4. 📅 **Line Chart: Year-wise Correlation Between COVID Metrics**

- Computes and displays year-wise correlation among:
  - `Cases Rate - Total`
  - `Hospitalizations Rate - Total`
  - `Deaths Rate - Total`

### 5. 📉 **Regression Plot: Case Rate Trend Over Time**

- Linear regression line over case rates by date
- Highlights how cases changed over time

---

## 🛠️ Libraries Used

- `pandas` for data manipulation
- `numpy` for numerical operations
- `scipy.stats` for outlier detection
- `matplotlib.pyplot` and `seaborn` for visualization
- `datetime` for date handling

---

## 📂 File Output

- Cleaned dataset is saved as `cleaned_dataset.csv`

---

## 📌 Requirements

Make sure to install the following Python packages before running the code:

```bash
pip install pandas numpy matplotlib seaborn scipy

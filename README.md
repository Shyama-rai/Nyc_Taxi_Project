# 🚕 NYC Taxi Ecosystem Investigation
## Data Analytics & Visualization Lab Exam — Jan & Feb 2024

---

## 🔢 Roll No Math (last 4 digits: 0379)
- W=0, X=3, Y=7, Z=9 → Sum = 19 → Digital root = 10 → **R = 1**
- f(x) = x³/3 − x² + 0·x = x³/3 − x²
- f'(x) = x² − 2x = x(x−2) = 0
- **Critical points: x=0 and x=2 → January & February 2024**

---

## 📁 Files in This Repository

| File | Description |
|------|-------------|
| `NYC_Taxi_Investigation.ipynb` | **Main Jupyter Notebook** — All 7 Acts |
| `nyc_taxi_jan_feb_2024.csv` | NYC Taxi dataset (Jan–Feb 2024, 80,000 trips) |
| `README.md` | This file |

---

## 🚀 How to Run

1. Open VS Code
2. Open the folder containing these files
3. Open `NYC_Taxi_Investigation.ipynb`
4. Click **Run All** (▶▶ button at the top)
5. All charts will appear inline in the notebook

**Required libraries** (install once in terminal):
```bash
pip install pandas numpy matplotlib seaborn scipy
```

---

## 📊 What Each Act Does

| Act | Topic | Method |
|-----|-------|--------|
| Act 1 | Critical Point Math | Calculus, matplotlib |
| Act 2 | Data Cleaning | Pandas, quality audit |
| Act 3 | Hypothesis Testing | Welch t-test, scipy |
| Act 4 | Time Patterns | Hourly/daily aggregation, seaborn |
| Act 5 | Policy Simulation | Fare elasticity model |
| Act 6 | Misinterpretation | Correct vs wrong analysis |
| Act 7 | Final Summary | Conclusions & limitations |

---

## 🗄️ SQL Queries
Full PostgreSQL queries are printed in the **SQL section** of the notebook (Act 6 area). They cover:
- Table creation & CSV loading
- Data quality checks (Act 2)
- Weekend vs weekday analysis (Act 3)
- Hourly & monthly aggregation (Act 4)
- Fare simulation query (Act 5)

---

## 📊 PowerBI Instructions
Export the following CSVs from the notebook output, then load into PowerBI:
1. Import `nyc_taxi_jan_feb_2024.csv` directly into PowerBI
2. Create calculated column: `trip_duration_min = DATEDIFF(MINUTE, [tpep_pickup_datetime], [tpep_dropoff_datetime])`
3. Filter: fare_amount > 0, trip_distance > 0, passenger_count > 0
4. Build visuals: Line chart (trips by date), Bar (hourly volume), Map (by LocationID), Card (revenue)

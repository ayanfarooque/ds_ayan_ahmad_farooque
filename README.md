# Trader Behavior Insights – Data Science Assignment

This repository contains the complete analysis for the **Trader Behavior Insights** assignment, focusing on the relationship between trader performance and market sentiment (Fear vs Greed) using Hyperliquid trade data and the Bitcoin Fear & Greed Index.

---

## 📁 Project Structure


```
ds_ayan_ahmad_farooque/
├── notebook_1.ipynb         # Main Google Colab notebook (EDA + analysis)
├── csv_files/               # Intermediate or processed datasets
│   ├── historical_data.csv
│   └── fear_greed_index.csv
├── outputs/                 # Saved plots and visualizations
│   └── *.png
├── ds_report.pdf            # Final summarized insights and findings
└── README.md                # Project setup and usage instructions
```

---
## 📊 Datasets Used

1. **Hyperliquid Historical Trade Data**
	- Granularity: Trade-level
	- Key fields: account, side, size_usd, closed_pnl, timestamps
	- Nature: High-frequency, multi-account trading data

2. **Bitcoin Fear & Greed Index**
	- Granularity: Daily
	- Fields: date, classification, numeric index value
	- Sentiment labels normalized to: `Fear`, `Greed`

---

## ⚙️ Environment & Requirements

All analysis was performed using **Google Colab**.

### Python Version
- Python 3.x (default Colab environment)

### Required Libraries
The following libraries are used (all pre-installed in Colab):

- pandas
- numpy
- matplotlib
- seaborn

No additional installation steps are required.

---

## ▶️ How to Run the Analysis

1. Open **Google Colab**
2. Upload `notebook_1.ipynb`
3. Upload the required CSV datasets:
	- `historical_data.csv`
	- `fear_greed_index.csv`
4. Run the notebook cells sequentially from top to bottom

All preprocessing, feature engineering, analysis, and visualization steps are fully contained within the notebook.

---

## 🔧 Methodology Overview

- Trade timestamps and sentiment dates are normalized and aligned at the **date level**
- Trades without sentiment alignment are excluded from sentiment-based analysis
- Extreme sentiment labels are collapsed into `Fear` and `Greed`
- Due to absence of explicit leverage data, **USD exposure–normalized metrics** are used as risk proxies
- Analysis focuses on:
  - Fear vs Greed performance comparison
  - Trader skill segmentation
  - Contrarian behavior analysis

---

## 📈 Outputs

- Key visualizations are saved in the `outputs/` directory
- Final summarized insights are documented in `ds_report.pdf`

---

## 📌 Notes

- Approximately **17% of total trades** align with available sentiment data due to differences in dataset coverage
- All conclusions are derived from the sentiment-aligned subset
- The project is fully reproducible using the provided notebooks and datasets

---

## 📬 Contact

**Candidate:** Ayan Farooque  
**Role Applied:** Junior Data Scientist – Trader Behavior Insights

---
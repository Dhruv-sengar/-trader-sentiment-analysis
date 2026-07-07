<div align="center">
  <h1>📊 Trader Performance vs Market Sentiment</h1>
  <p><em>An analytical deep-dive into how Bitcoin market sentiment drives trader behavior and profitability on Hyperliquid.</em></p>
  
  [![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
  [![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
  [![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg?logo=pandas)](https://pandas.pydata.org/)
  [![Primetrade.ai](https://img.shields.io/badge/Assignment-Primetrade.ai-success.svg)](#)
</div>

<hr />

## 📖 Overview
This project serves as a **Data Science/Analytics Intern Assignment** for **Primetrade.ai**. It aligns historical trader execution data from Hyperliquid with the daily Bitcoin Fear & Greed Index to uncover powerful behavioral and performance insights based on prevailing market conditions.

We explore critical questions:
- *Do traders perform better in fear or greed regimes?*
- *How does directional bias (% long trades) and trade sizing shift across market sentiments?*
- *Are frequent, high-turnover traders more susceptible to sentiment-driven drawdowns than infrequent traders?*

---

## 📁 Project Structure

The repository is thoughtfully organized for reproducibility:

```text
📦 trader-sentiment-analysis
 ┣ 📂 data             # Raw CSV datasets (Fear/Greed index & Historical trades)
 ┣ 📂 notebooks        # The core analytical Jupyter Notebook (main.ipynb)
 ┣ 📂 outputs          # Generated visual charts (.png) and summary tables (.csv)
 ┣ 📂 src              # Reusable helper scripts (e.g., automated notebook generator) 
 ┣ 📜 README.md        # Project documentation (You are here!)
 ┣ 📜 writeup.md       # Detailed methodology, insights, and actionable strategy rules
 ┗ 📜 requirements.txt # Python dependencies
```

---

## 🚀 Setup & Execution

### 1. Environment Setup
Install the required Python libraries. It is recommended to use a virtual environment.
```bash
pip install -r requirements.txt
```

### 2. Data Provisioning
Ensure your raw datasets are placed into the `/data` directory:
- `fear_greed_index.csv` (Bitcoin Market Sentiment)
- `historical_data.csv` (Hyperliquid Historical Trader Data)

### 3. Run the Analysis
Launch the Jupyter Notebook to explore the code, visualizations, and modeling:
```bash
jupyter notebook notebooks/main.ipynb
```
*Note: Execute all cells in `main.ipynb` to dynamically regenerate the insights. Output tables and charts will be automatically saved to the `/outputs` folder.*

---

## 💡 Key Highlights
- **Data Engineering**: Robust timestamp alignment and accurate directional bias extraction (filtering strictly for `Open Long` and `Open Short`).
- **Visual Analytics**: Clear, publication-ready visual arrays comparing PnL, Win Rates, and behavioral metrics across sentiment regimes.
- **Predictive Modeling**: A bonus Random Forest classifier designed to predict next-day profitability using lag features and one-hot-encoded sentiment states.
- **Actionable Output**: Data-backed strategy recommendations to adapt trading rules (position sizing, stop-losses, and frequency) based on whether the market is in Fear or Greed.

---
<div align="center">
  <i>Developed for the Primetrade.ai Data Science Internship.</i>
</div>

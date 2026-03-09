# Interest Rate Risk and Bond Market Analysis

This project processes and visualizes bond market data to analyze how changes in the **Federal Funds Rate** influence bond returns, duration risk, and market sensitivity across different asset classes including corporate bonds and Treasury Inflation-Protected Securities (TIPS).

---

## Setup

Create the conda environment and install dependencies:
conda env create -f environment.yml
conda activate bond-interest-dashboard

---

## Project Structure

data/
wrds_bond_returns.csv # WRDS bond-level dataset (returns, duration, yield)
rates_monthly.csv # Monthly interest rate data including Federal Funds Rate
tips.csv # Treasury / TIPS dataset

code/
preprocessing.py # Data cleaning and merging scripts
analysis.py # Generates summary statistics and charts

app.py # Streamlit dashboard for interactive visualization
environment.yml # Conda environment configuration
requirements.txt # Python package requirements
README.md # Project documentation


---

## Usage

Run the Streamlit dashboard:

streamlit run app.py


The dashboard will load the datasets and generate interactive visualizations including:

- Duration vs bond return scatter plot
- Average bond returns by duration bucket over time
- Heatmap of bond returns during tightening periods
- Relationship between Federal Funds Rate changes and bond returns

---

## Data Sources

This project combines three datasets:

1. **WRDS Bond Returns Dataset**
   - Bond-level returns, yields, duration, and maturity information

2. **Interest Rate Dataset**
   - Monthly Federal Funds Rate and Treasury yield curve measures

3. **CRSP Treasury / TIPS Dataset**
   - Treasury securities including inflation-protected bonds

---

## Policy Relevance

Understanding how bond markets respond to interest rate changes is important for assessing **financial stability risks** during periods of monetary tightening. This project explores how duration exposure amplifies the sensitivity of bond prices to monetary policy shocks.

---

## Authors

Lisa Liang  
Siwei Chen







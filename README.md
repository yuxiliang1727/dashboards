# dashboards
# Interest Rate Risk and Bond Market Sensitivity

This project analyzes how changes in the Federal Funds Rate influence bond returns and interest rate risk across different asset classes.

## Research Question

How do changes in the Federal Reserve's policy rate affect bond prices and returns across different maturities and durations?

## Data Sources

This project uses three datasets:

1. **WRDS Bond Returns Dataset**
   - Corporate and treasury bond data
   - Variables include price, yield, duration, maturity, and credit rating

2. **Interest Rate Dataset**
   - Monthly interest rate data including Federal Funds Rate
   - Treasury yield curve information

3. **CRSP Treasury / TIPS Dataset**
   - Treasury securities and inflation-protected securities
   - Includes yield, duration, and return data

## Visualization Dashboard

The Streamlit dashboard includes:

- Duration vs bond return scatter plot
- Time series of returns by duration bucket
- Heatmap of bond sensitivity during tightening periods
- Bubble chart comparing Federal Funds rate changes with bond returns

## Running the App

Install dependencies:

```bash
conda env create -f environment.yml
conda activate bond-interest-dashboard

streamlit run app.py

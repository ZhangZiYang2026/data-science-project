# US State-level Unemployment Rate and National Delinquency Analysis (2000-2025)

## 1. Problem / Research Question
How did unemployment rates across US states evolve from 2000 to 2025, and what were the differences in the impact of major economic shocks (like the 2008 Financial Crisis and the 2020 COVID-19 pandemic)? Furthermore, this project explores the descriptive co-movement between state unemployment rates and the national credit card delinquency rate.

## 2. Dataset Source and Usage Permissions
- **State Unemployment Data**: US Bureau of Labor Statistics (BLS). Excel file: `SeriesReport-20261019050857_3cedaf.xlsx`. Publicly available data, open for educational and analytical use.
- **National Delinquency Data**: Federal Reserve Board. CSV file: `DRCCLACBS.csv`. Publicly available data.
- **Sensitive Info Check**: No personal or restricted data is included. All data used is aggregated at the state or national level.

## 3. Methods and Tools
- **Language**: Python 3.10
- **Libraries**: Pandas (data manipulation), Matplotlib & Seaborn (data visualization).
- **Method**: 
  1. Data cleaning: Extracting FIPS codes, mapping to state names, and pivoting monthly data to annual averages.
  2. Visualization: Generating heatmaps for time-series trends, violin plots for cross-sectional distribution analysis, and dual-axis line charts for correlation analysis.
  3. Statistical Analysis: Calculating the Pearson correlation coefficient between mean state unemployment and national delinquency.

## 4. Key Findings and One Limitation
### Key Findings
- **Economic Shocks**: Unemployment spiked significantly across all states during the 2008-2010 Great Recession and the 2020 COVID-19 pandemic.
- **State Disparities**: States like Nevada and Michigan experienced much higher peaks, while states like North Dakota and South Dakota remained relatively stable.
- **Co-movement**: There is a moderate positive correlation (Pearson r ≈ 0.346) between the annual mean state unemployment rate and the national credit card delinquency rate, suggesting macroeconomic conditions strongly influence consumer credit health.

### Limitation
- This analysis relies on aggregated state-level and national-level data. It does not capture individual-level or industry-specific variations (e.g., tourism vs. manufacturing) that ultimately drive both unemployment and credit delinquency.

## 5. How to Run the Analysis

### Prerequisites
- Python 3.10 or higher
- Ensure all data files (`SeriesReport-20261019050857_3cedaf.xlsx`, `DRCCLACBS.csv`) are placed in the same directory as the Jupyter Notebook.

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/[你的GitHub用户名]/data-science-project.git
   cd data-science-project

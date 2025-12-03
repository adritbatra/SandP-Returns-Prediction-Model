# 📈 S&P 500 Returns Prediction Model

**Predicting Stock Market Returns Using Economic Indicators**

This project uses machine learning to predict S&P 500 year-over-year returns based on key economic indicators and monetary policy conditions.

---

## 🎯 Project Overview

Can we predict stock market performance using economic data? This analysis explores the relationship between S&P 500 returns and various macroeconomic factors including inflation, unemployment, monetary policy, and recession indicators.

### Key Question
How do inflation, unemployment, monetary stance, and recession status affect stock market returns?

---

## 📊 Data Sources

The analysis uses monthly data from multiple economic indicators:

- **S&P 500 Index** - Stock market performance
- **CPI (Consumer Price Index)** - Inflation measurement
- **Unemployment Rate** - Labor market health
- **Federal Funds Rate** - Central bank policy rate
- **R-star (Neutral Rate)** - Natural interest rate estimate
- **M2 Money Supply** - Monetary supply measure
- **Housing Starts** - Real estate market activity
- **Recession Indicator** - Economic downturn periods
- **Inflation Expectations** - 1-year forward expectations

---

## 🔧 Methodology

### Data Processing
1. **Data Cleaning** - Standardized date formats and variable names
2. **Feature Engineering** - Created year-over-year change metrics
3. **Monetary Stance Classification** - Categorized Fed policy as:
   - **Accommodative** - Rates below neutral rate
   - **Neutral** - Rates near neutral rate
   - **Restrictive** - Rates above neutral rate

### Models Built

#### 1. Linear Regression Models
- **Basic Model** - Simple linear relationships
- **Interaction Model** - Captures variable interactions
- **Polynomial Model** - Non-linear relationships

#### 2. Random Forest Model
- **500 trees** for robust predictions
- **Feature importance analysis** to identify key drivers
- **Cross-validation** for model evaluation

---

## 📈 Key Findings

### Visualizations Created

1. **Housing Starts by Monetary Stance**
   - Distribution across recession periods
   - Impact of policy on real estate

2. **CPI vs Unemployment Relationship**
   - Phillips curve analysis
   - Colored by recession status

3. **S&P 500 Returns by Monetary Policy**
   - Boxplot analysis
   - Performance during different policy stances

4. **Average Returns Analysis**
   - Bar chart comparing returns
   - Grouped by policy and recession

---

## 🛠️ Technologies Used

### R Packages
- **tidymodels** - Machine learning framework
- **tidyverse** - Data manipulation and visualization
- **ggplot2** - Data visualization
- **randomForest** - Random forest implementation
- **lubridate** - Date handling
- **readxl** - Excel file reading

### Analysis Tools
- **R Markdown** - Reproducible research
- **RStudio** - Development environment

---

## 📁 Project Structure

```
├── Predicting_S_P_500_Returns.Rmd    # Main analysis file
├── data/
│   ├── CPI.csv                       # Inflation data
│   ├── Unemployment_Rate.csv         # Labor market data
│   ├── Fed_Funds.csv                 # Interest rate data
│   ├── SPX.csv                       # S&P 500 data
│   ├── Housing_Starts.csv            # Housing data
│   ├── M2SL.csv                      # Money supply data
│   ├── Recession.csv                 # Recession indicators
│   ├── Neutral_Rate.xlsx             # R-star estimates
│   └── 1_Year_Inflation_Expectations.csv
└── README.md                         # This file
```

---

## 🚀 Getting Started

### Prerequisites
- R (version 4.0+)
- RStudio (recommended)

### Installation

1. **Install required packages**:
```r
install.packages(c(
  "tidymodels",
  "tidyverse",
  "readxl",
  "lubridate",
  "dplyr",
  "ggrepel",
  "ggplot2",
  "randomForest"
))
```

2. **Download the data files** and place them in your working directory

3. **Open the R Markdown file** in RStudio

4. **Update file paths** to match your directory structure

5. **Run the analysis** by knitting the document or running chunks

---

## 📊 Model Performance

### Linear Regression (Interaction Model)
- **RMSE** - Root Mean Squared Error on test set
- **R²** - Variance explained by the model

### Random Forest Model
- **Feature Importance** - Identifies key predictors
- **Out-of-bag Error** - Model validation metric
- **Test Set Performance** - Final model evaluation

---

## 🎓 Key Insights

1. **Monetary Policy Matters**
   - Stock returns vary significantly by Fed policy stance
   - Accommodative policy generally supports higher returns

2. **Recession Impact**
   - Strong negative impact on S&P 500 returns
   - Combined with monetary stance for better predictions

3. **Inflation-Unemployment Trade-off**
   - Classic Phillips curve relationship observed
   - Interactive effects with stock returns

4. **Economic Indicators**
   - Unemployment changes are a strong predictor
   - CPI year-over-year changes show clear patterns
   - Housing starts reflect economic confidence

---

## 📝 Model Variables

### Target Variable
- **S&P 500 YoY (%)** - Year-over-year percentage return

### Predictor Variables
- **CPI YoY (%)** - Inflation rate
- **Unemployment YoY (%)** - Labor market change
- **Recession** - Binary indicator (YES/NO)
- **Monetary Stance** - Fed policy position
- **Housing Starts** - New construction activity

---

## 🔍 Analysis Workflow

1. **Data Import** → Load all economic datasets
2. **Data Cleaning** → Standardize and format data
3. **Feature Engineering** → Create YoY metrics and policy indicators
4. **Data Merging** → Combine all sources by date
5. **Exploratory Analysis** → Visualize relationships
6. **Model Building** → Train linear and tree-based models
7. **Model Evaluation** → Compare performance metrics
8. **Feature Importance** → Identify key drivers

---

## 📌 Future Enhancements

- [ ] Add more economic indicators (VIX, bond yields)
- [ ] Implement time series models (ARIMA, GARCH)
- [ ] Include sector-specific analysis
- [ ] Add sentiment analysis from news/social media
- [ ] Create interactive dashboard
- [ ] Expand to other market indices

---

## 📖 References

- Federal Reserve Economic Data (FRED)
- Bureau of Labor Statistics (BLS)
- Federal Reserve Board
- S&P Dow Jones Indices

---

## 📄 License

This project is for educational and research purposes.

---

## 👤 Author

**Adrit Batra**

---

## 🤝 Contributing

Suggestions and improvements are welcome! Feel free to:
- Report issues
- Suggest new features
- Improve model performance
- Add new visualizations

---

**📊 Understanding markets through data analysis**

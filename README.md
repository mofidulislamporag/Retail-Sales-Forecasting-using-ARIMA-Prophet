# Retail-Sales-Forecasting-using-ARIMA-Prophet

## 📊 Project Overview

This project implements a comprehensive retail sales forecasting system using time series analysis and machine learning models. The goal is to predict future sales based on historical data to support business planning, inventory management, and resource allocation.

## 🎯 Business Problem

Retail businesses need accurate sales forecasts to:
- Optimize inventory levels
- Plan marketing campaigns
- Allocate resources efficiently
- Set realistic sales targets
- Identify seasonal trends and patterns

## 📈 Dataset

**File:** `https://www.kaggle.com/datasets/tanayatipre/store-sales-forecasting-dataset/data`

**Features:**
- Order Date: Transaction dates (2014-2017)
- Sales: Total sales amount
- Category: Product categories (Furniture, etc.)
- Quantity: Number of items sold
- Profit: Profit from each transaction
- Customer demographics and geographic information

**Dataset Characteristics:**
- Time period: 2014-2017
- ~800-900 transactions
- Daily granularity
- Multiple product categories

## 🛠️ Technical Approach

### Models Implemented

1. **ARIMA (AutoRegressive Integrated Moving Average)**
   - Traditional time series forecasting
   - Handles trend and seasonality
   - Multiple parameter combinations tested

2. **Facebook Prophet**
   - Advanced forecasting procedure
   - Automatic seasonality detection
   - Handles holidays and special events
   - Robust to missing data

### Methodology

```
Data Collection → EDA → Preprocessing → Model Training → Evaluation → Forecasting
```


## 📋 Implementation Steps

### Step 1: Data Loading & Exploration
- Load dataset and understand structure
- Basic statistics and data quality checks
- Date range analysis

### Step 2: Data Preprocessing
- Convert dates to datetime format
- Handle missing values
- Aggregate data to monthly level
- Create time series structure

### Step 3: Exploratory Data Analysis (EDA)
- Sales trends over time
- Seasonal patterns
- Category-wise analysis
- Statistical properties

### Step 4: Time Series Analysis
- Stationarity testing (ADF test)
- Autocorrelation analysis (ACF/PACF)
- Seasonal decomposition

### Step 5: Model Training
- Data splitting (80% train, 20% test)
- ARIMA parameter optimization
- Prophet model configuration
- Model fitting

### Step 6: Model Evaluation
- Performance metrics (MAE, RMSE, MAPE)
- Residual analysis
- Model comparison
- Visualization of predictions

### Step 7: Forecasting
- Future sales predictions
- Confidence intervals
- Business insights generation

## 📊 Key Metrics & Evaluation

### Performance Metrics Used:
- **MAE (Mean Absolute Error)**: Average absolute difference
- **RMSE (Root Mean Square Error)**: Penalizes larger errors
- **MAPE (Mean Absolute Percentage Error)**: Relative error measure

### Model Comparison:
| Model | MAE | RMSE | MAPE | Best For |
|-------|-----|------|------|----------|
| ARIMA | 6565.29 | 8493.99 | 32.41% | Short-term forecasts |
| Prophet | 4026.71 | 4428.18 | 19.88% | Seasonal patterns |

Best Performing Model: Prophet with MAE: 4026.71

## 📈 Results & Insights

### Key Findings:
1. **Seasonal Patterns**: Clear monthly/quarterly seasonality detected
2. **Trend Analysis**: [Upward/Downward/Stable] sales trend identified
3. **Best Performing Model**: [ARIMA/Prophet] based on evaluation metrics
4. **Forecast Accuracy**: [X]% MAPE on test data

### Business Insights:
- Peak sales months: [Months]
- Low sales periods: [Months]
- Recommended inventory planning strategy
- Marketing campaign timing suggestions

## 🎯 Usage

### For Business Users:
1. Run the notebook to generate sales forecasts
2. Review seasonal patterns for planning
3. Use forecasts for inventory management
4. Monitor model performance regularly

### For Data Scientists:
1. Experiment with different model parameters
2. Add external variables (holidays, promotions)
3. Extend to category-level forecasting
4. Implement rolling retraining


## ⚠️ Limitations & Considerations

### Current Limitations:
- Limited historical data (3 years)
- Sparse daily data requires aggregation
- No external variables included
- Single-store focus (can be extended to multiple locations)

### Recommendations for Improvement:
- Collect more historical data
- Include promotional calendar
- Add macroeconomic indicators
- Implement model retraining pipeline



## 👥 Authors

- [Md mafidul islam]



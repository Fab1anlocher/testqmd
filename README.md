# Credit Risk Management: Predictive Modeling Analysis

## Overview

This repository contains a comprehensive analysis of credit risk data aimed at developing predictive models to estimate the likelihood of companies defaulting on loans. The analysis leverages a real-world dataset with **15,045 observations** across **24 variables**.

## Project Objectives

The primary objectives of this work are to:

1. **Analyze Financial Data**: Examine comprehensive financial metrics from 15,045 companies
2. **Identify Risk Factors**: Determine key indicators associated with loan defaults
3. **Enable Risk Assessment**: Provide insights for more accurate lending decisions
4. **Support Predictive Modeling**: Create a foundation for machine learning models
5. **Promote Responsible Lending**: Contribute to prudent lending practices in the financial industry

## Repository Contents

### Data Files

- **`data_final_stand.csv`**: Main dataset containing 15,045 observations across 24 variables
  - Sample Size: 15,045 companies
  - Features: 24 variables including financial ratios, days metrics, and performance indicators
  - Target Variable: `status` (1 = default, 0 = non-default)

- **`Description of variables.jpg`**: Visual reference showing detailed descriptions of all variables in the dataset

### Analysis Files

- **`credit_risk_analysis.qmd`**: Comprehensive Quarto Markdown document containing:
  - Data loading and exploration
  - Descriptive statistics
  - Visualization of key patterns
  - Correlation analysis
  - Insights for credit risk prediction

## Dataset Variables

The dataset includes **24 variables** organized into the following categories:

### 1. Financial Ratios (16 variables)
- `ratio001` through `ratio030` (selected ratios)
- Various financial health and performance indicators

### 2. Days Metrics (3 variables)
- **DIO** (Days Inventory Outstanding): Measures inventory management efficiency
- **DPO** (Days Payable Outstanding): Indicates payment terms and cash management
- **DSO** (Days Sales Outstanding): Reflects accounts receivable efficiency

### 3. Performance Metrics (1 variable)
- **turnover**: Business revenue/turnover metric

### 4. Target Variable (1 variable)
- **status**: Loan default indicator
  - `1` = Company defaulted on loan
  - `0` = Company did not default

### 5. Additional Ratios (4 variables)
- `ratio036`, `ratio037`, `ratio039`, `ratio040`
- Supplementary financial indicators

For detailed variable descriptions, refer to the `Description of variables.jpg` file.

## How to Use This Analysis

### Prerequisites

To render and run the Quarto analysis, you need:

1. **R** (version 4.0 or higher)
2. **Quarto** (latest version recommended)
3. **R Packages**:
   - tidyverse
   - knitr
   - kableExtra
   - corrplot
   - ggplot2
   - scales
   - gridExtra

### Installation

1. **Install R**: Download from [r-project.org](https://www.r-project.org/)

2. **Install Quarto**: Download from [quarto.org](https://quarto.org/docs/get-started/)

3. **Install Required R Packages**:
   ```r
   install.packages(c("tidyverse", "knitr", "kableExtra", "corrplot", 
                      "ggplot2", "scales", "gridExtra"))
   ```

### Running the Analysis

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Fab1anlocher/testqmd.git
   cd testqmd
   ```

2. **Render the analysis to HTML**:
   ```bash
   quarto render credit_risk_analysis.qmd
   ```

3. **Render to PDF** (requires LaTeX):
   ```bash
   quarto render credit_risk_analysis.qmd --to pdf
   ```

4. **Open in RStudio** (alternative):
   - Open `credit_risk_analysis.qmd` in RStudio
   - Click the "Render" button
   - Select output format (HTML/PDF)

### Output Files

After rendering, you'll get:
- **`credit_risk_analysis.html`**: Interactive HTML report with embedded visualizations
- **`credit_risk_analysis.pdf`**: PDF version (if rendered to PDF)

## Analysis Structure

The Quarto analysis document includes:

### 1. Introduction
- Project overview and objectives
- Dataset description

### 2. Data Loading and Setup
- Library imports
- Data loading from CSV

### 3. Exploratory Data Analysis
- Dataset structure overview
- Variable summary tables
- Summary statistics for all variables

### 4. Target Variable Analysis
- Distribution of loan defaults
- Visualization of default rates
- Default vs non-default comparison

### 5. Missing Values Analysis
- Completeness check
- Missing data visualization (if any)

### 6. Distribution Analysis
- Financial ratios distributions by default status
- Days metrics analysis (DIO, DPO, DSO)
- Turnover analysis

### 7. Correlation Analysis
- Correlation matrix of all variables
- Correlation with target variable
- Identification of key predictive features

### 8. Key Insights and Findings
- Summary of analysis results
- Implications for credit risk management
- Recommendations for predictive modeling

## Key Features

✓ **Comprehensive Analysis**: Covers all 24 variables in detail  
✓ **Visual Insights**: Multiple visualizations for better understanding  
✓ **Statistical Rigor**: Detailed descriptive statistics and correlation analysis  
✓ **Reproducible**: Fully documented Quarto workflow  
✓ **Professional Output**: Publication-ready HTML and PDF reports  
✓ **Data Quality**: Complete dataset with no missing values  

## Use Cases

This analysis is valuable for:

1. **Financial Institutions**: Assess loan application risk
2. **Risk Managers**: Monitor portfolio health
3. **Data Scientists**: Build predictive models
4. **Researchers**: Study credit risk patterns
5. **Students**: Learn credit risk analysis techniques

## Next Steps

Based on this exploratory analysis, potential next steps include:

1. **Feature Engineering**: Create additional derived variables
2. **Model Development**: Build predictive models (logistic regression, random forest, etc.)
3. **Model Validation**: Implement cross-validation and performance metrics
4. **Deployment**: Create a scoring system for new loan applications
5. **Monitoring**: Establish KPIs for ongoing model performance

## Contributing

Contributions to improve the analysis are welcome! Please feel free to:
- Report issues
- Suggest enhancements
- Submit pull requests

## License

This project is available for educational and research purposes.

## Contact

For questions or feedback, please open an issue in this repository.

---

**Note**: This analysis provides insights based on historical data. Actual lending decisions should incorporate additional factors and comply with applicable regulations and institutional policies.

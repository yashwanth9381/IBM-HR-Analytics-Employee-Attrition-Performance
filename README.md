# 📊 IBM HR Analytics - Employee Attrition Analysis

<div align="center">

![Python](https://img.shields.io/badge/python-v3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/pandas-v1.3.0+-orange.svg)
![Matplotlib](https://img.shields.io/badge/matplotlib-v3.4.0+-green.svg)
![Seaborn](https://img.shields.io/badge/seaborn-v0.11.0+-red.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

*A comprehensive data analysis project to understand employee attrition patterns and identify key factors influencing workforce turnover.*

</div>

## 🎯 Project Overview

This project analyzes IBM's HR dataset to uncover insights about employee attrition patterns. Using Python and statistical analysis, we examine various factors that contribute to employee turnover, helping HR teams make data-driven decisions for better retention strategies.

### 🔍 What This Project Does

- **Analyzes** employee attrition rates across different demographics
- **Identifies** key factors contributing to employee turnover
- **Visualizes** patterns in workforce data through comprehensive charts
- **Provides** actionable insights for HR decision-making

## 📋 Dataset Features

The IBM HR Analytics dataset includes **35 columns** with the following key features:

### Employee Demographics
- `Age` - Employee age
- `Gender` - Male/Female
- `MaritalStatus` - Single/Married/Divorced
- `DistanceFromHome` - Distance from home to office

### Employment Details
- `Department` - Sales, Research & Development, Human Resources
- `JobRole` - Specific job positions
- `YearsAtCompany` - Total years with the company
- `YearsInCurrentRole` - Years in current position
- `Attrition` - **Target Variable** (Yes/No)

### Performance & Satisfaction
- `JobSatisfaction` - Job satisfaction rating
- `WorkLifeBalance` - Work-life balance rating
- `PerformanceRating` - Employee performance score
- `JobInvolvement` - Level of job involvement

### Compensation
- `MonthlyIncome` - Monthly salary
- `HourlyRate` - Hourly wage rate
- `StockOptionLevel` - Stock option level

## 🛠️ Technologies Used

| Technology | Purpose | Version |
|------------|---------|---------|
| **Python** | Main programming language | 3.8+ |
| **Pandas** | Data manipulation and analysis | 1.3.0+ |
| **NumPy** | Numerical computing | 1.21.0+ |
| **Matplotlib** | Data visualization | 3.4.0+ |
| **Seaborn** | Statistical data visualization | 0.11.0+ |
| **Jupyter** | Interactive development | 1.0.0+ |

## 🚀 Quick Start

### Prerequisites
```bash
Python 3.8 or higher
pip package manager
```

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ibm-hr-analytics.git
   cd ibm-hr-analytics
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Download the dataset**
   - Place `IBM HR Analytics Data.csv` in the project root directory
   - Update the file path in the code if necessary

4. **Run the analysis**
   ```bash
   python "IBM HR ANALYTICS.py"
   ```

## 📊 Key Analysis Components

### 1. Data Quality Assessment
- **Duplicate Check**: Identifies and removes duplicate records
- **Missing Values**: Comprehensive null value analysis
- **Data Types**: Validates and corrects data types

### 2. Exploratory Data Analysis
- **Descriptive Statistics**: Summary statistics for all variables
- **Distribution Analysis**: Understanding data distributions
- **Correlation Analysis**: Relationships between variables

### 3. Attrition Analysis
- **Overall Attrition Rate**: Company-wide turnover percentage
- **Demographic Breakdown**: Attrition by age, gender, department
- **Tenure Analysis**: Average years before leaving

### 4. Custom Functions
```python
def calculate_attrition_rate(df, column):
    """
    Calculate attrition rate for any categorical variable
    """
    # Implementation details in the code
```

## 📈 Key Visualizations

### 1. Attrition Rate Distribution
- Bar chart showing percentage of employees who left vs stayed
- Annotated with precise percentages

### 2. Employee Demographics
- **Age Distribution**: Histogram with KDE overlay
- **Gender Distribution**: Count plot by gender
- **Department Distribution**: Employee count by department

### 3. Attrition Patterns
- **Age-based Attrition**: KDE plot showing density by age
- **Gender-based Attrition**: Bar plot comparing attrition rates
- **Department-wise Analysis**: Comparative attrition rates

## 📊 Sample Results

```
📈 Key Metrics:
├── Overall Attrition Rate: 16.12%
├── Average Tenure: 7.01 years
├── Most Affected Age Group: 25-35 years
└── Highest Risk Department: Sales
```

## 🔍 Analysis Methodology

### Step 1: Data Preprocessing
```python
# Load and examine data
df = pd.read_csv("IBM HR Analytics Data.csv")
print(f"Dataset shape: {df.shape}")
print(f"Duplicates: {df.duplicated().sum()}")
print(f"Missing values: {df.isnull().sum().sum()}")
```

### Step 2: Attrition Rate Calculation
```python
# Calculate overall attrition rate
attrition_rate = df['Attrition'].value_counts(normalize=True)
print(f"Attrition Rate: {attrition_rate['Yes']*100:.2f}%")
```

### Step 3: Demographic Analysis
```python
# Custom function for demographic attrition analysis
def analyze_attrition_by_demographic(df, column):
    # Implementation in main script
    pass
```

## 📁 Project Structure

```
IBM-HR-Analytics/
│
├── 📄 IBM HR ANALYTICS.py          # Main analysis script
├── 📊 IBM HR Analytics Data.csv    # Dataset (not in repo)
├── 📋 README.md                    # Project documentation
├── 📝 requirements.txt             # Python dependencies
├── 📊 visualizations/              # Generated plots
│   ├── attrition_rate.png
│   ├── demographics.png
│   └── attrition_patterns.png
├── 📈 reports/                     # Analysis reports
│   └── hr_analytics_report.pdf
└── 🔧 utils/                       # Utility functions
    └── helper_functions.py
```

## 🎯 Key Insights

### 1. Attrition Patterns
- **16.12%** overall attrition rate
- **Younger employees** (25-35) show higher attrition
- **Sales department** has highest turnover

### 2. Gender Analysis
- Slight differences in attrition rates between genders
- Need for targeted retention strategies

### 3. Tenure Insights
- Average tenure of **7.01 years**
- Critical retention period identified in first 2 years

## 📊 Business Impact

### Cost Implications
- **Recruitment costs**: $15,000 per replacement
- **Training investment**: $10,000 per new hire
- **Productivity loss**: 3-6 months per departure

### Potential Savings
- **20% reduction** in attrition could save $2.5M annually
- **Improved retention** increases team productivity
- **Better planning** reduces recruitment urgency

## 🔮 Future Enhancements

### Phase 1: Advanced Analytics
- [ ] **Machine Learning Models** for attrition prediction
- [ ] **Survival Analysis** for time-to-attrition
- [ ] **Feature Engineering** for better insights

### Phase 2: Interactive Dashboard
- [ ] **Streamlit Dashboard** for real-time analysis
- [ ] **Plotly Integration** for interactive visualizations
- [ ] **Automated Reporting** with scheduled updates

### Phase 3: Predictive Capabilities
- [ ] **Risk Scoring** for individual employees
- [ ] **Early Warning System** for high-risk employees
- [ ] **Recommendation Engine** for retention strategies

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to the branch (`git push origin feature/amazing-feature`)
5. **Open** a Pull Request

### Contribution Guidelines
- Follow PEP 8 style guidelines
- Add comments for complex functions
- Include unit tests for new features
- Update documentation as needed

## 📄 Requirements

```txt
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
warnings>=0.1.0
```

## 📞 Contact & Support

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://linkedin.com/in/yourprofile)
[![Email](https://img.shields.io/badge/Email-Contact-red)](mailto:your.email@example.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/yourusername)

</div>

**Project Maintainer**: Yaswanth Rosannagari 
**Email**: yaswanth8460@gmail.com
**LinkedIn**: [https://www.linkedin.com/in/yashwanthrosannagari123/]  

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **IBM** for providing the comprehensive HR Analytics dataset
- **Python Community** for excellent data science libraries
- **Kaggle** for hosting the dataset and providing a platform for analysis
- **Contributors** who helped improve this project

## 📊 Dataset Source

The dataset used in this project is the **IBM HR Analytics Employee Attrition & Performance** dataset, which contains fictional data created by IBM data scientists.

- **Source**: IBM Watson Analytics
- **Size**: 1,470 employee records
- **Features**: 35 columns
- **Target Variable**: Attrition (Yes/No)

## 🔗 Related Projects

- [Employee Satisfaction Analysis](https://github.com/yourusername/employee-satisfaction)
- [HR Dashboard with Streamlit](https://github.com/yourusername/hr-dashboard)
- [Predictive Analytics for HR](https://github.com/yourusername/hr-predictive-analytics)

---

<div align="center">

**⭐ If you found this project helpful, please give it a star! ⭐**

*Last updated: January 2025*

</div>

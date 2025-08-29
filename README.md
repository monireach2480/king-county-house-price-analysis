# King County House Sales Analysis

A comprehensive data analysis project examining house sales in King County, Washington (including Seattle) using Python and machine learning techniques.

## 📊 Project Overview

This project analyzes house sale prices in King County from May 2014 to May 2015, implementing various data science techniques including data wrangling, exploratory data analysis, and predictive modeling using linear regression and Ridge regression.

## 🎯 Objectives

- Perform comprehensive data analysis on real estate data
- Clean and preprocess housing data with missing values
- Explore relationships between house features and prices
- Build and evaluate multiple regression models
- Compare model performance using different techniques

## 📋 Dataset

The dataset contains **21 features** describing house characteristics:

| Feature | Description |
|---------|-------------|
| `price` | House sale price (target variable) |
| `bedrooms` | Number of bedrooms |
| `bathrooms` | Number of bathrooms |
| `sqft_living` | Square footage of living space |
| `sqft_lot` | Square footage of the lot |
| `floors` | Number of floors |
| `waterfront` | Waterfront view (binary) |
| `view` | Quality of view |
| `condition` | Overall condition rating |
| `grade` | Overall grade (King County grading system) |
| `sqft_above` | Square footage above ground |
| `sqft_basement` | Square footage of basement |
| `yr_built` | Year built |
| `yr_renovated` | Year renovated |
| `zipcode` | ZIP code |
| `lat` | Latitude coordinate |
| `long` | Longitude coordinate |
| `sqft_living15` | Living room area in 2015 |
| `sqft_lot15` | Lot size area in 2015 |

## 🔧 Technologies Used

- **Python 3.x**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical data visualization
- **Scikit-learn** - Machine learning models and preprocessing

## 📈 Analysis Steps

### 1. Data Import & Exploration
- Load and examine the dataset structure
- Analyze data types and basic statistics
- Identify missing values

### 2. Data Wrangling
- Remove unnecessary columns (`id`, `Unnamed: 0`)
- Handle missing values in `bedrooms` and `bathrooms` using mean imputation
- Clean and prepare data for analysis

### 3. Exploratory Data Analysis
- **Floor Distribution**: Count houses by number of floors
- **Price Outliers**: Compare waterfront vs non-waterfront properties
- **Correlation Analysis**: Examine relationship between features and price
- **Feature Relationships**: Visualize sqft_above vs price correlation

### 4. Model Development
- **Simple Linear Regression**: Single feature models
- **Multiple Linear Regression**: Multi-feature prediction
- **Pipeline Implementation**: Scaled polynomial feature transformation

### 5. Model Evaluation
- **Ridge Regression**: Regularized linear regression
- **Polynomial Features**: Second-order polynomial transformation
- **Cross-validation**: Model performance assessment

## 📊 Key Findings

- **sqft_above** shows strong positive correlation with house prices
- Houses **without waterfront views** have more price outliers
- **Multiple features** significantly improve prediction accuracy
- **Polynomial feature transformation** enhances model performance
- **Ridge regression** helps prevent overfitting with multiple features

## 🚀 Model Performance

| Model Type | R² Score | Description |
|------------|----------|-------------|
| Single Feature (sqft_living) | ~0.4935 | Basic linear regression |
| Multiple Features | ~0.6576 | Linear regression with 11 features |
| Pipeline (Scaled + Polynomial) | ~0.7515 | Advanced preprocessing |
| Ridge Regression | ~0.6575 | Regularized model |
| Ridge + Polynomial | ~0.7005 | Best generalization |

## 📁 Project Structure

```
king-county-house-analysis/
├── House_Sales_in_King_Count_USA.ipynb
├── README.md
├── data/
│   └── kc_house_data_NaN.csv
├── visualizations/
│   ├── waterfront_boxplot.png
│   ├── sqft_above_regplot.png
│   └── correlation_matrix.png
└── models/
    ├── linear_regression_model.pkl
    ├── ridge_regression_model.pkl
    └── polynomial_pipeline.pkl
```

## 🔍 Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/king-county-house-analysis.git
   cd king-county-house-analysis
   ```

2. **Install required packages**:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```

3. **Run the Jupyter notebook**:
   ```bash
   jupyter notebook House_Sales_in_King_Count_USA.ipynb
   ```

## 📋 Requirements

```python
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=1.0.0
jupyter>=1.0.0
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [Len Monireach](https://github.com/monireach2480)
- LinkedIn: [Len Monireach](https://www.linkedin.com/in/len-monireach/)

## 🙏 Acknowledgment
- IBM Developer Skills Network for the original dataset and problem framework
- King County, Washington for providing the housing data
- Scikit-learn community for excellent machine learning tools

---

⭐ **Star this repository if you found it helpful!** ⭐
# Pusula Data Science Intern Case Study

**Name:** Tugce  
**Surname:** Sandikli  
**Email:** tugcesandikli@gmail.com

## Project Overview

This project contains a comprehensive analysis of a physical medicine & rehabilitation dataset with 2235 observations and 13 features. The main objective is to conduct in-depth Exploratory Data Analysis (EDA) and prepare the data for potential predictive modeling with **TedaviSuresi (Treatment Duration in Sessions)** as the target variable.

## Objectives

- **Primary Goal:** Make the data model-ready around the target variable `TedaviSuresi`
- **Secondary Goals:** 
  - Perform comprehensive EDA
  - Clean and preprocess the data
  - Handle missing values and outliers
  - Create meaningful features
  - Provide actionable insights

## Dataset Description

| Column | Description |
|--------|-------------|
| HastaNo | Anonymized patient ID |
| Yas | Age |
| Cinsiyet | Gender |
| KanGrubu | Blood type |
| Uyruk | Nationality |
| KronikHastalik | Chronic conditions (comma-separated list) |
| Bolum | Department/Clinic |
| Alerji | Allergies (may be single or comma-separated) |
| Tanilar | Diagnoses |
| TedaviAdi | Treatment name |
| **TedaviSuresi** | **Treatment duration in sessions (TARGET VARIABLE)** |
| UygulamaYerleri | Application sites |
| UygulamaSuresi | Application duration |

## How to Run the Code

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl
```

### Execution
1. Clone this repository:
   ```bash
   git clone https://github.com/tugcesandikli/Pusula_Tugce_Sandikli
   cd Pusula_Tugce_Sandikli
   ```

2. Place the data file `Talent_Academy_Case_DT_2025.xlsx` in the project directory

3. Run the main analysis:
   ```bash
   python pusula_case_study.ipynb
   ```

### Expected Output Files
- `model_ready_data.csv` - Clean dataset ready for modeling
- `processed_full_data.csv` - Complete processed dataset with all features
- Multiple visualization plots during execution

## Analysis Pipeline

### 1. Data Loading & Initial Exploration
- Dataset loading and basic info
- Column type identification
- Initial data quality assessment
- **Target variable (TedaviSuresi) deep dive**

### 2. Comprehensive EDA
- Missing value analysis with visualizations
- **Target variable distribution and statistics**
- Demographic analysis (Age, Gender, Blood Group, Nationality)
- Medical analysis (Departments, Treatments, Chronic Diseases, Diagnoses)
- Feature relationships and correlations

### 3. Data Preprocessing
- **Missing value handling** (Median for numeric, Mode for categorical)
- **Feature engineering** (Age groups, Numeric extractions, Count features)
- **Categorical encoding** (Label encoding with cardinality handling)
- **Outlier detection and treatment** (IQR method with capping)
- **Feature scaling** (StandardScaler for numeric features)

### 4. Model-Ready Dataset Preparation
- Feature selection for modeling
- Final data cleaning
- Target variable preparation
- Export clean datasets

## Key Findings

### Target Variable Analysis (TedaviSuresi)
- **Data Type:** String values like "10 Seans", "15 Seans", etc.
- **Processing:** Extracted numeric session counts for modeling
- **Distribution:** [Will be populated after running analysis]
- **Quality:** [Missing values and outliers handled]

### Demographics Insights
- **Age Distribution:** [To be filled after analysis]
- **Gender Split:** [To be filled after analysis]  
- **Blood Groups:** [Most common types identified]

### Medical Insights
- **Top Departments:** [Most frequent departments]
- **Common Treatments:** [Most prescribed treatments]
- **Chronic Diseases:** [Most prevalent conditions]

## 🛠️ Technical Implementation

### Libraries Used
```python
- pandas: Data manipulation and analysis
- numpy: Numerical computations
- matplotlib: Data visualization
- seaborn: Statistical visualizations
- scikit-learn: Preprocessing tools (LabelEncoder, StandardScaler, Imputers)
```

### Code Structure
- **Modular Design:** Object-oriented approach with separate classes
- **DataLoader:** Handles data loading and initial exploration
- **EDAAnalyzer:** Comprehensive exploratory data analysis
- **DataPreprocessor:** Data cleaning and preprocessing pipeline
- **Pipeline Integration:** End-to-end automated workflow

### Data Quality Measures
- **Missing Value Strategy:** Intelligent imputation based on data type
- **Outlier Handling:** IQR-based detection with capping (not removal)
- **Feature Engineering:** Domain-specific feature creation
- **Encoding Strategy:** Adaptive approach based on cardinality

## Modeling Readiness

The final dataset is prepared for various modeling approaches:

### Suitable Models for Target Prediction:
1. **Regression Models:**
   - Linear Regression
   - Random Forest Regressor
   - Gradient Boosting
   - XGBoost

2. **Classification Models** (if converting to categories):
   - Logistic Regression
   - Random Forest Classifier
   - SVM

### Features Ready for Modeling:
- Scaled numeric features
- Encoded categorical features  
- Engineered features (counts, groups)
- No missing values
- Outliers handled

## File Structure

```
Pusula_Tugce_Sandikli/
├── README.md                          # This documentation
├── pusula_case_study.ipynb              # Main analysis script
├── Talent_Academy_Case_DT_2025.xlsx  # Original dataset
├── model_ready_data.csv              # Clean dataset for modeling
├── processed_full_data.csv           # Complete processed dataset
└── requirements.txt                  # Python dependencies
```

## Future Enhancements

1. **Advanced Feature Engineering:**
   - Text mining on chronic diseases and diagnoses
   - Interaction features between departments and treatments
   - Temporal features if date information available

2. **Model Development:**
   - Cross-validation framework
   - Model comparison and selection
   - Performance metrics evaluation
   - Feature importance analysis

3. **Additional Analysis:**
   - Clustering analysis for patient segmentation
   - Association rule mining for treatment patterns
   - Statistical significance testing

## Contact

For questions or clarifications about this analysis:

**Email:** [Your Email]  
**Project Repository:** `https://github.com/tugcesandikli/Pusula_Tugce_Sandikli`

## Notes

- Ensure the Excel file `Talent_Academy_Case_DT_2025.xlsx` is in the same directory
- The analysis generates several plots - close each plot window to continue execution
- Processing time depends on system specifications (estimated: 2-5 minutes)
- All preprocessing steps are logged to console for transparency


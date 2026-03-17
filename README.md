# Obesity Analysis in the United States

A comprehensive data visualization project analyzing nutrition, physical activity, and obesity trends across U.S. states from 2011 to 2023. This project uses the Behavioral Risk Factor Surveillance System (BRFSS) dataset to explore the relationship between dietary habits, physical activity levels, and obesity rates.

## Overview

This project investigates adult obesity patterns in the United States by analyzing behavioral risk factors including nutrition and physical activity. The analysis covers all U.S. states and includes demographic breakdowns by age, education, sex, income, and race/ethnicity.

## Project Structure

```
obesity-analysis-in-us/
├── Nutrition__Physical_Activity__and_Obesity_-_Behavioral_Risk_Factor_Surveillance_System.csv
│   └── Raw dataset from CDC BRFSS
├── cleanning_data.ipynb
│   └── Data cleaning and preprocessing notebook
├── analysis_notebook.ipynb
│   └── Data analysis and visualization notebook
├── Data_Visualization_Presentation.pdf
│   └── Final presentation with visualizations and findings
└── cleaned/
    ├── cleaned_nutrition_obesity_data.csv
    ├── cleaned_states_overall.csv
    ├── cleaned_by_age.csv
    ├── cleaned_by_education.csv
    ├── cleaned_by_income.csv
    ├── cleaned_by_race.csv
    └── cleaned_by_sex.csv
```

## Data Source

The project uses data from the **Behavioral Risk Factor Surveillance System (BRFSS)**, a CDC surveillance system collecting behavioral health data from U.S. adults. The dataset includes:

- **Obesity / Weight Status**: Percentage of adults aged 18+ with obesity
- **Physical Activity**: Percentage of adults meeting physical activity guidelines
- **Fruits and Vegetables**: Percentage of adults consuming adequate fruits and vegetables

**Time Period**: 2011-2023
**Geographic Coverage**: All U.S. states
**Demographic Dimensions**: Age, Education, Sex, Income, Race/Ethnicity

## Key Research Questions

1. **What are the main trends in adult obesity rates across U.S. states over time?**
   - Temporal analysis of obesity prevalence
   - Regional variations in obesity rates
   - Year-over-year changes

2. **How have average physical activity levels and dietary habits changed from 2011 to 2023?**
   - Physical activity trends across states
   - Fruits and vegetables consumption patterns
   - Correlation between lifestyle factors and obesity

3. **Which demographic groups are most affected by obesity?**
   - Age-based obesity analysis
   - Income-level disparities
   - Education-based trends
   - Sex-based differences
   - Race/ethnicity considerations

## Files Description

### Raw Data
- **Nutrition__Physical_Activity__and_Obesity_-_Behavioral_Risk_Factor_Surveillance_System.csv**
  - Original dataset with 110,882 rows
  - Contains 35 columns including demographic stratifications
  - Data spanning multiple years and all U.S. territories

### Notebooks

#### cleanning_data.ipynb
Data preprocessing pipeline that:
- Loads and explores the raw BRFSS dataset
- Filters data for the 2011-2023 period
- Selects relevant classes (Obesity, Physical Activity, Fruits and Vegetables)
- Removes non-state territories, keeping only the 50 U.S. states
- Handles missing values and data inconsistencies
- Creates stratified datasets for different demographic dimensions
- Exports cleaned datasets to the `cleaned/` folder

#### analysis_notebook.ipynb
Comprehensive analysis with 14+ visualizations:
- Overall obesity trends (2011-2023)
- Regional obesity rate comparisons
- Physical activity and dietary habits trends
- Demographic breakdowns by age, education, income, sex, and race
- Geographic heatmaps showing state-level obesity variations
- Correlation analysis between lifestyle factors and obesity

### Cleaned Data Files
- **cleaned_nutrition_obesity_data.csv**: Main cleaned dataset with all records
- **cleaned_states_overall.csv**: Aggregated data at state level
- **cleaned_by_age.csv**: Obesity data stratified by age groups
- **cleaned_by_education.csv**: Obesity data stratified by education level
- **cleaned_by_income.csv**: Obesity data stratified by income brackets
- **cleaned_by_race.csv**: Obesity data stratified by race/ethnicity
- **cleaned_by_sex.csv**: Obesity data stratified by sex

### Output
- **Data_Visualization_Presentation.pdf**: 18-slide presentation containing key findings and visualizations

## Getting Started

### Prerequisites
- Python 3.7+
- Jupyter Notebook
- Required packages:
  - pandas
  - numpy
  - matplotlib
  - geopandas
  - plotly (optional, for interactive visualizations)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/dangkien1311/Obesity-analysis-in-US.git
cd Obesity-analysis-in-US
```

2. Install required packages:
```bash
pip install pandas numpy matplotlib geopandas
```

3. Open and run the notebooks:
```bash
jupyter notebook
```

### Workflow

1. **Data Cleaning**: Run `cleanning_data.ipynb` first to preprocess the raw dataset
2. **Analysis**: Run `analysis_notebook.ipynb` to generate visualizations and insights
3. **Review**: Check the `Data_Visualization_Presentation.pdf` for executive summary

## Key Findings

The analysis reveals:

- Adult obesity rates in the U.S. have remained relatively stable between 30-35% from 2011 to 2023
- Regional disparities exist, with certain regions showing higher obesity prevalence
- Physical activity levels and fruit/vegetable consumption show varied trends over time
- Demographic factors (age, income, education, race) significantly influence obesity rates
- Income and education levels show inverse correlation with obesity rates
- Geographic variations suggest environmental and socioeconomic factors influence obesity

## Technologies Used

- **Python 3**: Data processing and analysis
- **Pandas**: Data manipulation and aggregation
- **NumPy**: Numerical computations
- **Matplotlib**: Static visualizations
- **GeoPandas**: Geographic data analysis and mapping
- **Jupyter Notebook**: Interactive development environment

## Author

Trung Kien Dang

## License

This project uses publicly available BRFSS data from the CDC.

## References

- CDC Behavioral Risk Factor Surveillance System: https://www.cdc.gov/brfss/
- BRFSS Data: https://data.cdc.gov/
- CDC Obesity Prevention: https://www.cdc.gov/obesity/

## Contact

For questions or inquiries about this project, please contact the author or open an issue on GitHub.

---

Last Updated: March 2026

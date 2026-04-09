## Dataset 1: Customer Personality Analysis

### Cleaning Steps:
- Handled missing values in `Income` using median
- Removed duplicate rows
- Converted `Dt_Customer` to datetime format
- Standardized categorical variables (`Education`, `Marital_Status`)
- Removed constant columns (`Z_CostContact`, `Z_Revenue`)
- Created new features: `age`, `total_children`

### Output:
Cleaned dataset saved in:
data/processed/dataset1_clean.csv
# Dataset 1: Customer Personality Analysis

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


# Dataset 2: Medical Appointment No Shows

### Cleaning Steps:
- Handled missing values using appropriate checks (`.isnull()`)
- Removed duplicate rows
- Converted `scheduledday` and `appointmentday` to datetime format
- Removed timezone information from datetime columns
- Standardized column names (lowercase, underscores, no special characters)
- Converted `patientid` from scientific notation to string
- Standardized categorical variables (`gender`, `no_show`)
- Converted `no_show` to numeric (0 = No, 1 = Yes)
- Removed invalid values (e.g., negative `age`)
- Created new feature: `waiting_days` (difference between appointment and scheduled date)
- Adjusted `waiting_days` to remove time-based inconsistencies

### Output:
Cleaned dataset saved in:
data/processed/dataset2_clean.csv
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


# Dataset 3: Mall Customer Segmentation Data

### Cleaning Steps:
- Checked and handled missing values using `.isnull()`
- Removed duplicate rows
- Standardized column names (lowercase, removed spaces)
- Fixed data types for numerical columns (age, income, spending score)
- Standardized categorical values (`gender`)
- Renamed columns for better readability
- Checked for invalid or inconsistent values

### Output:
Cleaned dataset saved in:
data/processed/dataset3_clean.csv


# Dataset 4: Netflix Movies and TV Shows

### Cleaning Steps:
- Checked and handled missing values in `director`, `cast`, `country`, `rating`, and `date_added`
- Converted `date_added` to datetime format
- Removed duplicate rows
- Standardized column names (lowercase, underscores)
- Fixed data types for numerical columns
- Standardized categorical values (`type`, `country`)
- Processed `duration` column into numeric and categorical components
- Extracted additional features (`year_added`, `month_added`)

### Output:
Cleaned dataset saved in:
data/processed/dataset4_clean.csv



# Dataset 5: Sales Data

### Cleaning Steps:
- Removed unnecessary columns (`unnamed`)
- Converted `user_id` from float to integer
- Converted `time_stamp` to datetime format (day-first handled)
- Removed duplicate rows
- Standardized column names (lowercase, underscores)
- Standardized categorical values (`interaction_type`)
- Extracted new features: `year`, `month`, `day`

### Output:
Cleaned dataset saved in:
data/processed/dataset5_clean.csv
# Absenteeism Data Analysis

## Project Overview
In this project, I focused on cleaning and preprocessing absenteeism data to prepare it for further analysis. The dataset includes information like employee ID, department, absence duration, and reasons for absence. My goal was to improve data quality by addressing missing values, handling duplicates, and ensuring overall consistency.

## Data Cleaning Process

### 1. **Understanding the Data Structure**
- **Examine Data**: I began by exploring the dataset to understand the columns and their data types, such as employee ID, absence duration, and reasons for absence.
- **Data Dictionary**: Whenever possible, I referred to a feature descriptions file to clarify the meaning and relationships between variables.

### 2. **Cleaning Steps**

#### a. **Handle Missing Values**
- **Identify Missing Data**: I checked for null or missing values in the dataset.
- **Impute or Remove**: Depending on the situation, I either imputed missing values (using methods like mean or median) or removed rows/columns with excessive missing data.

#### b. **Detect and Remove Duplicates**
- **Check for Duplicates**: I ensured that there were no duplicate entries, particularly focusing on unique identifiers like employee ID.
- **Remove or Merge**: When duplicates were found, I either removed or merged them as appropriate.

#### c. **Correct Data Types**
- **Ensure Correct Data Types**: I made sure that data types were correctly assigned, such as treating dates as `datetime`, numerical values as floats or integers, and categorical variables as strings.
- **Convert Data Types**: If necessary, I converted values to their proper data types to ensure accuracy in the analysis.

### 3. **Outlier Detection**
- **Identify Outliers**: I detected any unusual values, such as extreme absence durations or negative values.
- **Handle Outliers**: For any outliers, I decided whether to remove, flag, or further investigate these data points.

### 4. **Ensure Data Consistency**
- **Standardize Categories**: I ensured that categories (e.g., absence reasons) were consistently applied throughout the dataset.
- **Logical Consistency**: I verified that dates and values made logical sense, such as ensuring that absence end dates came after start dates.

### 5. **Organize the Dataset**
- **Remove Redundant Columns**: I removed columns that didn’t contribute meaningfully to the analysis.
- **Rename Columns**: I standardized the column names for better readability.

### 6. **Address Specific Challenges**
- **Absence Reasons**: I ensured that the reasons for absence were clearly defined and consistently categorized (e.g., medical leave, vacation).
- **Absence Duration**: I made sure that the absence duration was measured consistently, either in days or hours.

### 7. **Final Verification**
- **Check for Anomalies**: Once the cleaning process was complete, I reviewed the dataset for any remaining issues, such as incorrect formatting or suspicious patterns.
- **Validate with Business Rules**: I cross-checked the cleaned data against relevant business rules (e.g., maximum allowed absence days) to ensure accuracy.

### 8. **Prepare for Further Analysis**
- **Document Cleaning Process**: Throughout the cleaning process, I kept detailed notes of all changes, such as how I handled missing values or removed columns.
- **Export Clean Dataset**: I saved the cleaned dataset as a CSV file, making it ready for further analysis.

## Files
- **Absences-from-work-with-pandas.ipynb**: The Jupyter notebook where I cleaned and processed the data.
- **absenteeism-data.csv**: The original dataset with raw absenteeism data (if included).
- **absenteeism-data-cleaned.csv**: The final cleaned dataset, ready for analysis (output).
- **feature descriptions.xlsx**: Description of columns and categories of reasons for absence of employees

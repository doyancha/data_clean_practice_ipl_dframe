# IPL Data Cleaning Practice

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-orange.svg)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **A comprehensive guide to cleaning IPL (Indian Premier League) cricket match data using Python and Pandas. Learn step-by-step data preprocessing techniques from importing data to exporting cleaned datasets.**

---

## 📋 Table of Contents

- [🎯 Overview](#-overview)
- [📊 Dataset Description](#-dataset-description)
- [🛠️ Prerequisites](#️-prerequisites)
- [🚀 Getting Started](#-getting-started)
- [📚 Notebook Sections](#-notebook-sections)
- [🔧 Data Cleaning Steps](#-data-cleaning-steps)
- [📁 Files in Repository](#-files-in-repository)
- [💡 Key Learnings](#-key-learnings)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)
- [👤 Author](#-author)

---

## 🎯 Overview

This repository demonstrates professional data cleaning techniques applied to IPL cricket match data. The project covers essential data preprocessing steps including handling missing values, data type conversions, column renaming, and feature engineering.

**Key Features:**
- ✅ Comprehensive data cleaning pipeline
- ✅ Step-by-step Jupyter notebook walkthrough
- ✅ Real-world IPL dataset (2008-2022)
- ✅ Professional code practices
- ✅ Detailed explanations and comments

---

## 📊 Dataset Description

The dataset contains IPL match data from 2008 to 2022 with the following information:
- Match details (date, venue, teams)
- Toss and match results
- Player information
- Umpire details
- Win margins and methods

**Original Dataset:** `ipl-matches.csv` (471KB, 950+ matches)  
**Cleaned Dataset:** `cleaned_ipl.csv` (Ready for analysis)

---

## 🛠️ Prerequisites

Before running this notebook, ensure you have the following installed:

- **Python 3.8+**
- **Pandas** - Data manipulation library
- **Jupyter Notebook** - For interactive coding
- **NumPy** (automatically installed with Pandas)

### Installation

```bash
# Install required packages
pip install pandas jupyter

# Or using conda
conda install pandas jupyter
```

---

## 🚀 Getting Started

1. **Clone the repository:**
   ```bash
   git clone https://github.com/doyancha/data_clean_practice_ipl_dframe.git
   cd data_clean_practice_ipl_dframe
   ```

2. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```

3. **Open the notebook:**
   - Navigate to `ipl_Data_cleaning_practice.ipynb`
   - Run cells sequentially to follow the cleaning process

4. **View results:**
   - Check `cleaned_ipl.csv` for the final cleaned dataset

---

## 📚 Notebook Sections

The Jupyter notebook is organized into logical sections covering the complete data cleaning pipeline:

### 1. 📥 Importing Libraries and DataFrame
- Import necessary Python libraries (Pandas)
- Load the IPL matches CSV file
- Initial data exploration with `df.head()`

### 2. 🔍 Observing the Columns
- Examine column names and structure
- Understand the dataset schema

### 3. ✏️ Renaming Columns for Better Understanding
- Rename columns for clarity (e.g., `MatchNumber` → `Match Number`)
- Improve readability of column headers

### 4. 🔍 Checking Null Values
- Identify columns with missing values
- Analyze null value patterns

### 5. 🗑️ Handling Missing Values - Strategic Row Removal
- Identify rows with extensive missing data
- Remove problematic rows to simplify cleaning process

### 6. 🏙️ Filling Missing City Values
- Extract city information from venue names
- Fill missing city data using venue parsing

### 7. 📏 Filling Missing Margin Values
- Handle numeric missing values in margin column
- Convert to appropriate data types

### 8. 🎯 Filling Missing Method Values
- Handle categorical missing values
- Use appropriate placeholder values

### 9. 📅 Date Processing and Feature Engineering
- Convert date strings to datetime objects
- Extract month and day information
- Create new temporal features

### 10. 🔄 Column Re-ordering
- Reorganize columns for better data flow
- Position related columns together

### 11. 🔧 Data Type Optimization
- Convert columns to appropriate data types
- Optimize memory usage and performance

### 12. 📆 Season Column Handling
- Split season ranges (e.g., "2008/09") into start/end years
- Handle different season formats
- Convert to integer types

### 13. 💾 Exporting Cleaned Data
- Save the processed dataset to CSV
- Ensure proper formatting for downstream analysis

---

## 🔧 Data Cleaning Steps

| Step | Operation | Description |
|------|-----------|-------------|
| 1 | **Import & Load** | Load CSV data into Pandas DataFrame |
| 2 | **Initial Inspection** | Check data types, shape, and basic statistics |
| 3 | **Column Renaming** | Improve column names for readability |
| 4 | **Null Value Analysis** | Identify and quantify missing data |
| 5 | **Row Removal** | Drop rows with excessive missing values |
| 6 | **Missing Value Imputation** | Fill missing values using domain knowledge |
| 7 | **Data Type Conversion** | Convert columns to appropriate types |
| 8 | **Feature Engineering** | Create new columns (Month, Day, Season Start/End) |
| 9 | **Column Reordering** | Organize columns logically |
| 10 | **Final Validation** | Ensure data quality and integrity |
| 11 | **Export** | Save cleaned data to new CSV file |

---

## 📁 Files in Repository

| File | Description | Size |
|------|-------------|------|
| `ipl_Data_cleaning_practice.ipynb` | Main Jupyter notebook with cleaning code | ~73KB |
| `ipl-matches.csv` | Original raw IPL match data | ~471KB |
| `cleaned_ipl.csv` | Processed and cleaned dataset | ~471KB |
| `README.md` | Project documentation | ~171B |

---

## 💡 Key Learnings

Through this project, you'll learn:

- **Data Import Techniques** - Loading CSV files with Pandas
- **Data Exploration** - Understanding dataset structure and content
- **Missing Data Handling** - Various strategies for dealing with null values
- **Data Type Management** - Converting between different data types
- **Feature Engineering** - Creating new features from existing data
- **Data Cleaning Best Practices** - Systematic approach to data preprocessing
- **Pandas Operations** - Advanced DataFrame manipulation techniques

---

## 🤝 Contributing

Contributions are welcome! Please feel free to:

- 🐛 **Report bugs** - Open issues for any problems
- 💡 **Suggest features** - Ideas for improving the cleaning process
- 📝 **Improve documentation** - Better explanations or examples
- 🔧 **Code improvements** - Optimize existing cleaning steps

### How to Contribute:
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Doyancha**  
- GitHub: [@doyancha](https://github.com/doyancha)
- Project: Data Cleaning Practice with IPL DataFrame

---

*⭐ Star this repository if you found it helpful!

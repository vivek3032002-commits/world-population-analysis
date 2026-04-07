# Pandas DataFrame Filtering: Boolean Indexing Tutorial

A practical demonstration of Boolean indexing techniques in Pandas using world population data (2026).

## 📋 Overview

This repository demonstrates two efficient approaches to filtering DataFrames using Boolean indexing—a fundamental technique for data analysis and business intelligence workflows.

## 🗃️ Dataset

- **File:** `world_population_by_country_2026.csv`
- **Records:** 233 countries
- **Key Column:** `Population_2026`

## 🔍 Filtering Techniques

### Method 1: Stored Boolean Condition
```python
import pandas as pd

# Load dataset
data = pd.read_csv('world_population_by_country_2026.csv', index_col=0)

# Create Boolean mask
is_huge = data['Population_2026'] > 190000000

# Apply filter
filtered_data = data[is_huge]
```

**Advantages:**
- Reusable condition across multiple operations
- Improved code readability
- Easy to modify thresholds

### Method 2: Direct Inline Filtering
```python
# Filter directly
filtered_data = data[data['Population_2026'] > 190000000]
```

**Advantages:**
- Concise syntax
- Ideal for one-time filters
- Common in exploratory analysis

## 💼 Business Use Cases

- **Customer Segmentation:** Filter high-value customers by revenue thresholds
- **Market Analysis:** Identify priority regions based on population or GDP
- **KPI Monitoring:** Extract records exceeding performance benchmarks
- **Risk Assessment:** Flag accounts above credit limit thresholds

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas
```

### Running the Code
```bash
python Filter_Dataset.ipynb
```

## 📊 Results

Both methods return identical DataFrames containing only countries with populations exceeding 190 million.

**Key Insight:** Boolean indexing creates a True/False mask that Pandas uses to select matching rows—efficient and scalable for large datasets.

## 📫 Connect

Feel free to reach out for collaboration or questions about data analysis workflows.

**LinkedIn:** www.linkedin.com/in/vivek-kannadasan

## 📄 License

This project is open source and available for educational purposes.v# Pandas DataFrame Filtering: Boolean Indexing Tutorial

A practical demonstration of Boolean indexing techniques in Pandas using world population data (2026).

## 📋 Overview

This repository demonstrates two efficient approaches to filtering DataFrames using Boolean indexing—a fundamental technique for data analysis and business intelligence workflows.

## 🗃️ Dataset

- **File:** `world_population_by_country_2026.csv`
- **Records:** 233 countries
- **Key Column:** `Population_2026`

## 🔍 Filtering Techniques

### Method 1: Stored Boolean Condition
```python
import pandas as pd

# Load dataset
data = pd.read_csv('world_population_by_country_2026.csv', index_col=0)

# Create Boolean mask
is_huge = data['Population_2026'] > 190000000

# Apply filter
filtered_data = data[is_huge]
```

**Advantages:**
- Reusable condition across multiple operations
- Improved code readability
- Easy to modify thresholds

### Method 2: Direct Inline Filtering
```python
# Filter directly
filtered_data = data[data['Population_2026'] > 190000000]
```

**Advantages:**
- Concise syntax
- Ideal for one-time filters
- Common in exploratory analysis

## 💼 Business Use Cases

- **Customer Segmentation:** Filter high-value customers by revenue thresholds
- **Market Analysis:** Identify priority regions based on population or GDP
- **KPI Monitoring:** Extract records exceeding performance benchmarks
- **Risk Assessment:** Flag accounts above credit limit thresholds

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas
```

### Running the Code
```bash
python Filter_Dataset.ipynb
```

## 📊 Results

Both methods return identical DataFrames containing only countries with populations exceeding 190 million.

**Key Insight:** Boolean indexing creates a True/False mask that Pandas uses to select matching rows—efficient and scalable for large datasets.

## 📫 Connect

Feel free to reach out for collaboration or questions about data analysis workflows.

**LinkedIn:** www.linkedin.com/in/vivek-kannadasan

## 📄 License

This project is open source and available for educational purposes.
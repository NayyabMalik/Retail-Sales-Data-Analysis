# Retail Sales Data Analysis

## Overview

This project performs exploratory data analysis (EDA) on a retail sales dataset to uncover insights into transaction patterns. Using Python, Pandas, Matplotlib, Seaborn, and Statistics, the project analyzes sales metrics such as product categories, prices, and quantities, demonstrating skills in data preprocessing, statistical analysis, and visualization for data science applications.

## Dataset

The dataset (`sales_data.csv.xls`) contains 100 retail transaction records with the following columns:

- **store_id**: Identifier for the store (e.g., Store 01, Store 15).
- **customer_id**: Unique customer identifier (e.g., Customer 1508).
- **product_id**: Unique product identifier (e.g., 53642.0).
- **product_category**: Product category (e.g., Toys, Movies, Books, Clothing).
- **date**: Transaction date and time (e.g., 4/1/07 8:09 AM).
- **amount**: Quantity purchased (1 to 9 units).
- **single_price**: Price per unit (ranging from 10.85 to 99.16).
- **transaction_id**: Unique transaction identifier (1 to 100).

## Features

- **Data Loading and Inspection**:
  - Loads the dataset using Pandas.
  - Displays the first few rows (`df.head()`) and summary statistics (`df.describe()`).
  - Checks for missing values (`df.isnull().sum()`), confirming no missing data.
- **Exploratory Data Analysis**:
  - Calculates statistical measures for `single_price`:
    - Mean: 55.61
    - Median: 55.21
    - Mode: 90.25
  - Visualizes the distribution of `amount` using a Matplotlib boxplot, revealing a median of 5 units and no significant outliers.
  - Explores relationships between `product_category` and `single_price` using a Seaborn scatterplot, identifying price variations across categories (e.g., Toys and Movies tend to have higher prices).
- **Tools and Libraries**:
  - Python: Pandas, Matplotlib, Seaborn, Statistics
  - Jupyter Notebook for interactive analysis and visualization

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/retail-sales-data-analysis.git
   cd retail-sales-data-analysis
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Place the `sales_data.csv.xls` file in the `data/` directory.

## Usage

1. Open the Jupyter Notebook:

   ```bash
   jupyter notebook Retail_Sales_Data_Analysis.ipynb
   ```

2. Update the file path in the notebook to point to your `data/sales_data.csv.xls` file (e.g., `./data/sales_data.csv.xls`).

3. Run all cells to:
   - Load and preprocess the dataset.
   - Compute statistical measures (mean, median, mode) for `single_price`.
   - Generate visualizations (boxplot for `amount`, scatterplot for `product_category` vs. `single_price`).

## Repository Structure

```
retail-sales-data-analysis/
├── data/
│   └── sales_data.csv.xls   # Retail sales dataset
├── Retail_Sales_Data_Analysis.ipynb  # Main notebook
├── README.md               # Project documentation
├── LICENSE                 # MIT License
```

## Requirements

Install the required libraries using:

```bash
pip install pandas matplotlib seaborn
```

## Notes

- The dataset has no missing values, ensuring reliable analysis.
- The boxplot of `amount` shows a range of 1 to 9 units, with a mean of 4.62 and a standard deviation of 2.47, indicating moderate variability in purchase quantities.
- The scatterplot suggests that product categories like Toys and Movies have higher `single_price` values compared to Books and Clothing.
- Future enhancements could include:
  - Analyzing sales trends over time by parsing the `date` column.
  - Visualizing total sales (`amount` × `single_price`) by store or category.
  - Applying clustering to group similar transactions or customers.
- The notebook uses a local file path (`C:\\Users\\PMLS\\Documents\\sales_data.csv.xls`). Update to a relative path (e.g., `./data/sales_data.csv.xls`) for portability.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For questions, contact nayyabm16@gmail.com or open an issue on GitHub.

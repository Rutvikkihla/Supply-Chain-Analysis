# Supply-Chain-Analysis

## Project Overview
This project explores and analyzes supply chain data using Jupyter Notebook. It applies data analysis and visualization techniques to identify patterns, trends, inefficiencies, and potential improvement opportunities in supply chain operations.

The project is useful for understanding inventory movement, demand patterns, order performance, supplier behavior, and overall supply chain efficiency.

## Objective
The main goal of this project is to analyze supply chain data and convert raw information into meaningful, actionable insights.

This project aims to:
- Understand supply chain performance
- Identify trends and patterns in the data
- Analyze demand and inventory behavior
- Detect potential delays or operational issues
- Present findings through clear charts and visualizations
- Support data-driven business decisions

## Tools and Technologies
- **Programming Language:** Python
- **Environment:** Jupyter Notebook
- **Libraries:** Pandas, NumPy, Matplotlib, and Seaborn
- **Development Tool:** Jupyter Notebook or JupyterLab
- **Data Source:** Supply chain dataset used within the notebook

## Dataset
The dataset contains supply chain-related information such as:
- Product details
- Order information
- Inventory quantities
- Sales or demand records
- Shipping information
- Supplier or warehouse details
- Delivery dates
- Transportation costs
- Revenue or sales values

Before analysis, the data is examined for missing values, duplicate records, incorrect formats, and outliers.

## Project Structure
```text
Supply-Chain-Analysis/
│
├── Supply Chain Analysis.ipynb
└── README.md
```

## Step-by-Step Process

### 1. Import Required Libraries
The required Python libraries are imported to perform data analysis and visualization.

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
```

### 2. Load the Dataset
The supply chain dataset is loaded into a Pandas DataFrame.

```python
df = pd.read_csv("data.csv")
df.head()
```

### 3. Review the Dataset
The dataset structure, column names, data types, and basic statistics are reviewed.

```python
df.info()
df.describe()
df.shape
```

### 4. Clean the Data
The data is cleaned to remove errors and prepare it for analysis.

Common cleaning tasks include:
- Handling missing values
- Removing duplicate rows
- Converting date columns
- Correcting incorrect data types
- Removing or handling outliers
- Standardizing column names

```python
df.drop_duplicates(inplace=True)
df.dropna(inplace=True)
```

### 5. Perform Exploratory Data Analysis
Exploratory Data Analysis helps discover patterns and relationships in the supply chain data.

Typical analysis includes:
- Sales and demand trends
- Product-wise performance
- Supplier performance
- Inventory levels
- Transportation costs
- Order and delivery patterns
- Regional or warehouse performance

### 6. Create Visualizations
Visualizations are used to present findings in an easy-to-understand format.

Examples:
- Line charts for demand trends
- Bar charts for product or supplier comparison
- Pie charts for category distribution
- Histograms for data distribution
- Heatmaps for correlation analysis
- Scatter plots for relationship analysis

```python
sns.set_theme(style="whitegrid")

plt.figure(figsize=(10, 6))
sns.barplot(data=df, x="Category", y="Sales")
plt.title("Sales by Category")
plt.xticks(rotation=45)
plt.show()
```

### 7. Analyze Supply Chain Insights
The final analysis identifies important findings, such as:
- High-performing and low-performing products
- Frequently delayed deliveries
- Products with high inventory levels
- Categories with strong or weak demand
- Cost-heavy transportation activities
- Potential opportunities to improve efficiency

### 8. Provide Recommendations
Based on the analysis, useful recommendations can be suggested, such as:
- Improve inventory planning
- Reduce delivery delays
- Optimize transportation costs
- Monitor low-demand products
- Strengthen supplier relationships
- Improve warehouse allocation
- Use demand trends for better forecasting

## Key Analysis Features
- Data cleaning and preprocessing
- Exploratory data analysis
- Trend analysis
- Statistical summary
- Data visualization
- Supply chain performance evaluation
- Business insight generation
- Practical recommendations

## How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/Rutvikkihla/Supply-Chain-Analysis.git
```

### 2. Open the Project Folder
```bash
cd Supply-Chain-Analysis
```

### 3. Install Jupyter Notebook
```bash
pip install jupyter
```

### 4. Install Required Libraries
```bash
pip install pandas numpy matplotlib seaborn
```

### 5. Start Jupyter Notebook
```bash
jupyter notebook
```

### 6. Open the Notebook
Open the project notebook from the Jupyter interface and run every cell from top to bottom.

## Example Insights
The notebook may reveal insights such as:
- Certain products generate higher sales than others
- Some suppliers or regions experience longer delivery times
- Specific periods show higher demand
- Excess inventory may increase storage costs
- Transportation cost varies by region or shipping method
- Demand forecasting can help improve stock planning

## Conclusion
This project demonstrates how supply chain data can be analyzed using Python and Jupyter Notebook. Through cleaning, exploratory analysis, and visualization, the project converts raw data into useful insights that can support inventory planning, cost reduction, supplier evaluation, and overall supply chain optimization.

## Future Scope
- Build a demand forecasting model
- Create an interactive dashboard
- Apply predictive analytics
- Predict delivery delays
- Implement inventory optimization
- Use machine learning for supplier risk analysis
- Monitor supply chain performance in real time

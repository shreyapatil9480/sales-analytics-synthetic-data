# Synthetic Sales Data Analysis Project

This project provides a **ready‑to‑use** repository for demonstrating business, program management, and data analysis skills. It includes a **synthetic sales dataset**, a **Jupyter notebook** with exploratory data analysis and predictive modeling, and supporting documentation so that it can be cloned and run out of the box.

## Dataset

The dataset (`synthetic_sales_data.csv`) contains 500 records of simulated retail transactions. Each record includes:

- **Date** – Date of transaction (January 2022 to December 2024)
- **Product_ID** – Unique identifier for each product
- **Product_Category** – Category such as Electronics, Clothing, Home & Kitchen, Sports, or Beauty
- **Customer_Age** – Age of the customer
- **Customer_Gender** – Gender (`Male`/`Female`)
- **Region** – Geographic region (`North`, `South`, `East`, `West`, `Central`)
- **Season** – Season of the transaction (`Winter`, `Spring`, `Summer`, `Autumn`)
- **Sales_Quantity** – Number of units sold
- **Unit_Price** – Price per unit (in USD)
- **Discount** – Discount applied (0–30 %)
- **Total_Sales** – Revenue after discount (computed)
- **Advertising_Spend** – Marketing expenditure for the sale
- **Cost_per_unit** – Cost price per unit
- **Profit** – Profit per transaction (computed)
- **Profit_Margin** – Profit as a fraction of Total Sales (computed)

The dataset is purely synthetic and is generated programmatically. It can be extended or regenerated using the script embedded in the notebook.

## Notebook (`analysis_notebook.ipynb`)

The Jupyter notebook guides users through:

1. **Loading and inspecting the dataset** to understand its structure and summary statistics.
2. **Exploratory data analysis (EDA)** using descriptive statistics and visualizations (histograms, box plots, correlation heatmap) to uncover patterns and relationships.
3. **Regression modeling** to predict total sales based on features. A simple linear regression model is built with one‑hot encoding for categorical variables. Performance is evaluated with RMSE and R².
4. **Classification modeling** to predict whether sales quantity is above the median. A logistic regression model is constructed, and results are assessed using accuracy and a classification report.
5. **Concluding insights** highlighting key findings and suggestions for future work.

You can run the notebook locally or in any Jupyter environment. Follow the usage instructions below.

## Usage

### Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/synthetic-sales-data-analysis.git
cd synthetic-sales-data-analysis
```

Replace `YOUR_USERNAME` with your GitHub username if you fork the repository.

### Set up a Virtual Environment (optional)

Create and activate a virtual environment to manage dependencies:

```bash
python3 -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### Install Dependencies

Install the required Python packages using `pip`:

```bash
pip install -r requirements.txt
```

### Run the Notebook

Start Jupyter Notebook or JupyterLab and open `analysis_notebook.ipynb`:

```bash
jupyter notebook
# or
jupyter lab
```

Execute the cells sequentially to reproduce the analysis and models. The notebook reads the dataset from `synthetic_sales_data.csv`, so ensure all files are in the same directory.

### Regenerating the Dataset

If you wish to generate a fresh synthetic dataset or extend the number of samples, modify the data‑generation section of the notebook accordingly. The dataset is created using NumPy and pandas, and additional features can be introduced to suit specific analysis needs.

## File Structure

```
├── analysis_notebook.ipynb   # Jupyter notebook with EDA and models
├── synthetic_sales_data.csv  # Synthetic dataset
├── requirements.txt          # List of Python dependencies
└── README.md                 # Project overview and instructions
```

## Dependencies

Key packages used in this project include:

- **pandas** – data manipulation
- **numpy** – numerical operations
- **matplotlib** & **seaborn** – data visualizations
- **scikit‑learn** – machine learning models and preprocessing

Refer to `requirements.txt` for the full list and versions. You can upgrade or pin versions as needed.

## Contributing

This repository is intended as a showcase and learning resource. Feel free to fork it, experiment with different models, add new visualizations, or expand the dataset. Pull requests are welcome if you have improvements or corrections.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

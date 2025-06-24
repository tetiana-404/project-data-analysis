# Product Data Analysis

## 📌 Project Brief

This project involves loading, cleaning, vizualizing and analyzing product data from a CSV file `hw20240224_Matched.csv`. The goal is to uncover insights into product characteristics such as pricing, category, color, and production timelines.

## 🎯 Objectives

- Load and inspect the dataset
- Clean missing or inconsistent data
- Check and enforce proper data types
- Perform basic exploratory data analysis
- Visualize insights using graphs
- Provide recommendations and document limitations

## 📁 Dataset Overview

- File: `hw20240224_Matched.csv`
- Columns: 41
- Records: 397
- Contains multilingual product descriptions, cost/pricing, dates, and category details

## 📂 Folder Structure

- `data/`: Raw dataset
- `src/`: Data cleaning scripts
- `notebooks/`: Jupyter notebook for exploration
- `presentation/`: PDF export of the final report
- `requirements.txt`: Python dependencies

## ▶️ How to Run

1. Clone the repository:
    ```bash
    git clone https://github.com/<your-username>/product-data-analysis.git
    cd product-data-analysis
    ```

2. Create a virtual environment and install dependencies:
    ```bash
    python -m venv env
    source env/bin/activate      # On Windows: env\Scripts\activate
    pip install -r requirements.txt
    ```

3. Launch the notebook:
    ```bash
    jupyter notebook notebooks/product_analysis.ipynb
    ```

## 📊 Tools & Libraries

- Python
- pandas
- numpy
- matplotlib / seaborn
- Jupyter Notebook

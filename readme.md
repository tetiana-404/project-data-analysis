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

## 🧱 Dataset Structure

| Column Name                   | Type        | Description                                 |
| ----------------------------- | ----------- | ------------------------------------------- |
| ProductAlternateKey           | Object      | Alternative product identifier              |
| WeightUnitMeasureCode         | Categorical | Unit of measurement for weight              |
| SizeUnitMeasureCode           | Categorical | Unit of measurement for size                |
| EnglishProductName            | Object      | Product name in English                     |
| SpanishProductName            | Object      | Product name in Spanish                     |
| FrenchProductName             | Object      | Product name in French                      |
| StandardCost                  | Float       | Cost to manufacture                         |
| FinishedGoodsFlag             | Boolean     | Indicates if product is finished            |
| Color                         | Categorical | Product color                               |
| SafetyStockLevel              | Int         | Minimum stock level before restocking       |
| ReorderPoint                  | Int         | Stock level that triggers reorder           |
| ListPrice                     | Float       | Product retail price                        |
| Size                          | Object      | Product size description                    |
| SizeRange                     | Object      | Range of available sizes                    |
| Weight                        | Float       | Product weight                              |
| DaysToManufacture             | Int         | Number of days to manufacture               |
| ProductLine                   | Categorical | Product line or category                    |
| DealerPrice                   | Float       | Wholesale price                             |
| Class                         | Categorical | Product classification                      |
| Style                         | Categorical | Product style                               |
| ModelName                     | Object      | Name of the product model                   |
| EnglishDescription            | Object      | Description in English                      |
| FrenchDescription             | Object      | Description in French                       |
| ChineseDescription            | Object      | Description in Chinese                      |
| ArabicDescription             | Object      | Description in Arabic                       |
| HebrewDescription             | Object      | Description in Hebrew                       |
| ThaiDescription               | Object      | Description in Thai                         |
| GermanDescription             | Object      | Description in German                       |
| JapaneseDescription           | Object      | Description in Japanese                     |
| TurkishDescription            | Object      | Description in Turkish                      |
| StartDate                     | Datetime    | Date when product became available          |
| EndDate                       | Datetime    | Date when product was discontinued (if any) |
| Status                        | Categorical | Product status (e.g., Active, Discontinued) |
| EnglishProductSubcategoryName | Object      | Subcategory name in English                 |
| SpanishProductSubcategoryName | Object      | Subcategory name in Spanish                 |
| FrenchProductSubcategoryName  | Object      | Subcategory name in French                  |

---

## 🧼 Data Cleaning Process

- 🧹 Dropped 6 fully empty columns
- 🔄 Replaced comma decimal separators and converted to float
-  Convert to datetime data types
-  Convert to category data types
- ❓ Filled missing **categorical** data 
- 🧮 Filled missing **numeric** data with column **medians**

---

## 📈 Exploratory Data Analysis (EDA)
- Generated descriptive statistics for numeric fields
- Created correlation heatmap to assess variable relationships
- Plotted histograms of:
  - Product `List Price`
  - `StandardCost` vs `ListPrice` vs `DealerPrice`
  - `Weight` and `DaysToManufacture`???????????????????

---

## 💡 Key Insights

- Significant gaps in weight data may affect shipping analytics
- Product pricing structures are consistent within subcategories

---

## ✅ Recommendations

- Ensure weight data is consistently entered for logistics
- Consider reviewing duplicate SKU imports during data entry
- Investigate outliers in pricing for premium products

---
 
## 📂 Folder Structure

- `data/`: Raw dataset
- `src/`: Data cleaning scripts
- `notebooks/`: Jupyter notebook for exploration
- `presentation/`: PDF export of the final report
- `requirements.txt`: Python dependencies

---

## ⚠️ Limitations

- No unique product IDs — duplicates were inferred
- Some missing values in key columns may skew analysis
- Currency for prices not specified — assume consistent

---

## 📊 Tools & Libraries

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

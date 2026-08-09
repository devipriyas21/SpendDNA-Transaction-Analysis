# SpendDNA – Personal Transaction Analysis

A Python-based transaction analysis tool that cleans messy bank/UPI data, extracts vendors, categorises spending, analyses spending patterns, detects anomalies, and generates a financial spending report.

## 📌 Project Overview

SpendDNA analyses six months of synthetic Indian bank/UPI transaction data and converts raw transaction records into meaningful financial insights.

The project covers:

- Transaction parsing and cleaning
- Vendor extraction and normalisation
- Spending category tagging
- Overall spending analysis
- Monthly spending trends
- Time-of-day spending patterns
- Anomaly detection using category-wise z-scores
- Spending archetype detection
- Final formatted financial report

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Google Colab / Jupyter Notebook

## 📊 Features

### 1. Transaction Parser
Cleans dates, amounts and transaction types and removes duplicate records.

### 2. Vendor Extractor
Converts messy transaction descriptions into canonical vendor names using dictionary-based keyword matching.

### 3. Category Tagger
Maps vendors into spending categories such as Food Delivery, E-commerce, Quick Commerce, Transport, Restaurants, Investments, Utilities and more.

### 4. Spending Overview
Calculates:

- Total credits
- Total debits
- Net savings
- Savings rate
- Total transactions
- Top spending categories
- Top vendors

### 5. Monthly Trend Analysis
Analyses spending across January–June and compares category-wise monthly spending.

### 6. Time-of-Day Analysis
Extracts the transaction hour and identifies spending patterns across different times of the day.

### 7. Anomaly Detection
Uses category-wise z-scores to identify unusually large transactions.

```text
z-score = (Amount - Category Mean) / Category Standard Deviation
### 8. Spending Archetype Detection

Identifies spending behaviours based on quantitative rules and assigns relevant spending archetypes to the transaction history.

Possible archetypes include:

- The Shopaholic
- The YOLO Spender
- The Foodie
- The Quick Commerce Junkie
- The Investor

A user can match multiple archetypes depending on their spending behaviour.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Google Colab / Jupyter Notebook

## 📊 Key Concepts

- Data cleaning and preprocessing
- Dictionary-based vendor mapping
- String manipulation
- Pandas DataFrames
- GroupBy and aggregation
- Pivot tables
- Datetime analysis
- Percentage calculations
- Category-wise statistical analysis
- Z-score based anomaly detection
- Conditional logic

## 🔒 Project Constraints

### Allowed

- Python fundamentals
- Lists, tuples, sets and dictionaries
- NumPy
- Pandas
- Datetime operations
- String methods
- `groupby()`
- `agg()`
- `pivot_table()`
- `transform()`
- `apply()`
- Basic mathematical and statistical calculations

### Not Used

- Regular expressions (`re`)
- Machine Learning libraries
- AI/ML/GenAI libraries
- Transaction parsing libraries
- External transaction datasets
- `scikit-learn`
- `scipy.stats`
- `statsmodels`
- `matplotlib`
- `seaborn`
- `plotly`

The z-score for anomaly detection is calculated manually using the required formula.

## 🤖 AI Assistance

AI was used as a learning and debugging aid during the development of this project.

It was used for:

- Understanding Pandas concepts
- Debugging errors
- Understanding programming logic
- Reviewing code structure

AI-assisted cells are marked inside the notebook with appropriate comments.

## ▶️ How to Run

### Google Colab

1. Open `SpendDNA_Devipriya_S.ipynb` in Google Colab.
2. Upload `rahul_transactions.csv` to the Colab session.
3. Run all cells from beginning to end.
4. View the final SpendDNA report.

### Jupyter Notebook

Install the required libraries:

```bash
pip install pandas numpy
Make sure `rahul_transactions.csv` is in the same folder as the notebook.

Then open the notebook and run all cells sequentially from the first cell to the last cell.

## 📁 Repository Structure

```text
SpendDNA-Personal-Transaction-Analysis/
│
├── SpendDNA_Devipriya_S.ipynb
├── rahul_transactions.csv
├── output_screenshot.png
└── README.md

## 🖼️ Sample Output

![SpendDNA Report](output_screenshot.png)

The screenshot shows the final formatted SpendDNA transaction analysis report.

## 🔐 Privacy

The project uses the provided synthetic transaction dataset.

No real personal bank or UPI statement is included in this repository.

## 👩‍💻 Author

**Devipriya S**

B.Tech Computer Science Engineering – Data Science  
Presidency University, Bengaluru

## 📚 Project

**SpendDNA – Week 2 Minor Project**  
The Unlox Academy

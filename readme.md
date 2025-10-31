# Bike Sales Analysis

A Jupyter Notebook project analyzing a bike company's sales data to identify high-revenue customers, high-value countries, profitable bike models, and seasonal sales patterns. The analysis uses Python (pandas, matplotlib, seaborn) to answer business questions and provide actionable recommendations.

Repository contents
- Bike Sales Analysis.ipynb — Jupyter Notebook containing the full analysis, visualizations and findings.
- (Dataset is not included in the repo) The notebook expects a CSV dataset (original path in the notebook: "C:\Users\osaze\OneDrive\Desktop\MySQL\Projects\Datasets\Sales Data for Bike Company.csv").

Key questions answered
- Who are the top customers (by age, age group)?
- Which countries have the highest revenue per order?
- Which bike models generate the most profit?
- When during the year do sales spike?

Summary of main findings
- United States generates the most total revenue.
- Australia and Germany have the highest revenue per order (strong purchasing power).
- Adults aged 35–64 generate the highest total revenue by age group.
- 28-year-olds are the top single-age revenue contributors, although 31-year-olds have the highest order counts — suggesting higher average order value for 28-year-olds.
- Road Bikes are the most profitable bike sub-category.
- Sales peak in December (holiday season).

Requirements
- Python 3.8+
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn

Install dependencies (example)
- Using pip:
  pip install pandas numpy matplotlib seaborn jupyter

How to run
1. Clone the repository:
   git clone https://github.com/moyez48/Bike-Sales-Analysis.git
2. Place the dataset CSV file in a local path and update the file path in the notebook cell that reads the CSV:
   df = pd.read_csv(r"<path-to-your>/Sales Data for Bike Company.csv")
3. Launch Jupyter and open the notebook:
   jupyter notebook
4. Open `Bike Sales Analysis.ipynb` and run the cells (or run them sequentially).

Notebook structure (high level)
- Data import and type conversions (Date to datetime).
- Exploratory analysis:
  - Revenue by age group and specific age.
  - Order counts by age group and age.
  - Revenue per order by country (used due to lack of unique customer IDs).
  - Top bike models by profit (filtering Product_Category == 'Bikes').
  - Monthly revenue trends to identify seasonal spikes.
- Visualizations using seaborn and matplotlib with in-notebook plots and printed summaries.

Notes & recommendations
- The notebook calculates "revenue per order" because the dataset lacks unique customer identifiers. If a unique customer ID becomes available, consider computing revenue per customer for more accurate lifetime value or per-customer comparisons.
- Consider adding:
  - Data validation and missing-value handling.
  - Automated environment setup via a requirements.txt or environment.yml.
  - A small sample dataset or synthetic data for reproducible demos.
  - Exporting summary tables or interactive visualizations (Plotly) for stakeholders.

Contact / Author
- Original notebook: Bike Sales Analysis.ipynb
- Notebook permalink:
  https://github.com/moyez48/Bike-Sales-Analysis/blob/32865c5ed06246834536dc6c0268dd5295424dc5/Bike%20Sales%20Analysis.ipynb

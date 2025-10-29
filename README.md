Bike Sales Analysis
A data-driven exploration of sales trends for a fictional bicycle company, designed to uncover high-revenue customers, top-performing markets, and product growth opportunities.

Project Overview
This project analyzes bicycle sales data to:
	Identify high-revenue customers and countries
	Highlight profitable product lines
	Reveal seasonal sales trends and key business opportunities
	Analysis is performed in a Jupyter Notebook using Python (Pandas, Matplotlib/Seaborn, etc.).

File Structuretext
Bike-Sales-Analysis/
├─ data/
│   └─ Sales Data for Bike Company.csv  # (Not included in this repository)
├─ Bike Sales Analysis.ipynb
├─ requirements.txt
└─ README.md

Bike Sales Analysis.ipynb — Main analysis notebook with data cleaning, EDA, and visualizations.

data/ — Directory for your dataset. (Must add file yourself.)

requirements.txt — Python dependencies.

Getting Started
Add the dataset: Place the sales data at data/Sales Data for Bike Company.csv. (Or, update the path in the notebook if you use a different location.)

Set up the Python environment (Windows PowerShell):

powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
Open and run the notebook:

powershell
jupyter notebook "Bike Sales Analysis.ipynb"
Run all cells, top-to-bottom.

If you’re on Mac/Linux, activate the virtual environment using . .venv/bin/activate instead of the PowerShell command.

Key Findings
The US leads in total revenue, while Australia and Germany deliver top revenue per order.

28-year-olds generate the highest total revenue by age; 31-year-olds are the largest group by order count.

Road Bikes bring in highest profits across categories.

December is the single peak sales month.

See the notebook for detailed charts and business takeaways.

Data Limitations
No unique Customer_ID: All "per customer" metrics are actually "per order" (i.e., per row in the dataset). This is clearly documented in both the notebook and README.

Metrics may change if unique IDs are added; adjust using .nunique() where relevant.

Reproducibility & Portability
Paths: Always use the data/ folder (relative path) to store the CSV, never hard-coded computer-specific paths.

Share clean notebooks: Remove large outputs before committing, or use nbstripout to keep version control lightweight.

License
This project is currently not licensed for redistribution or re-use. If you wish to open-source it, consider adding an MIT License or similar.

Contact
[Majesty Umoye on LinkedIn](https://www.linkedin.com/in/majestyumoye)


# **Two Decades of Educational Change: Global Enrollment Trends and Gender Gap Reduction, 2000–2020**

This repository contains data, analysis scripts, cleaned datasets, figures, and reports for a comprehensive analysis of global educational progress from 2000 to 2020. The project focuses on **regional convergence toward world average enrollment**, **gender parity trends**, and **education equity across primary, secondary, and tertiary levels**.

---

## **Project Structure**
```bash
qtm350-final-project/
│
├── data/               # Folder with raw and cleaned data
│
├── figures/            # Folder with figures generated for the report
│
├── scripts/            # Folder with code notebooks for cleaning, modeling, and analysis
│
├── final_report.qmd    # Quarto report
├── final_report.html   # Rendered HTML report
├── final_report.pdf    # Rendered PDF report
├── final_report_files/ # Folder for HTML dependencies
├── final_report_cache/ # Folder for Quarto cache
│
├── wdi_edu.db          # SQLite database
├── apa.csl             # Citation style file
├── references.bib      # References for citation
├── requirements.txt    # Python packages
└── README.md           # Project documentation
```

---

## **Installation**

### 1. Clone the repository

```bash
git clone https://github.com/yxyang05/qtm350-final-project.git
cd qtm350-final-project
```

### 2. Create and activate a virtual environment
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```
---

## **How to Run the Analysis**

### 1. Data Cleaning

Run the Jupyter notebook:
```bash
scripts/wdi_edu_data_cleaning.ipynb
```
This notebook performs the following:
- Imports the raw WDI education dataset  
- Cleans and filters for enrollment indicators, relevant years (2000-2020), and regions of interest
- Reshapes the data into long formats  
- Outputs (stored in the `data/` folder):
  - Raw dat CSV file (`wdi_edu.csv`)
  - Cleaned and filtered CSV files (`wdi_edu_filtered_long.csv`)

### 2. Data Analysis
Run the Jupyter notebook:
```bash
scripts/wdi_edu_analysis.ipynb
```
This notebook performs the various summary statistics...

### 3. Convergence & Statistical Analysis

Run the following notebooks:
```bash
scripts/"Education Convergence Analysis.ipynb"
scripts/"Gender Gap Analysis.ipynb"
```

Computed visualizations are stored in the `figures/` folder.
---

## **Render the Final Quarto Report**

Using Quarto and the terminal, run:
```bash
quarto render final_report.qmd --to html
quarto render final_report.qmd --to pdf
``` 
---

## Key Outputs

- **Figures:** Convergence trends, gender parity plots, regional comparisons  
- **Clean datasets:** Filtered table for modeling and analysis
- **SQLite database:** `wdi_edu.db`  
- **Final report:** Comprehensive results in HTML and PDF  

---

## Reproducibility Notes

- Set the working directory to the project root before running notebooks.  
- PDF rendering requires LaTeX installed.  
- All figures are generated from the `.ipynb` notebooks in `/scripts`.  

---

## References

- `references.bib` — citation entries  
- `apa.csl` — APA citation style for Quarto  

---

## Author

  - Annie Cao
  - Vicki Wang
  - Yan Yang
  - Gloria Wang

QTM 350 Final Project


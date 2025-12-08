# INSY6500_job_market_analysis
Repository exploring the https://www.kaggle.com/datasets/jakupymeraj/jobs-a-2025-dataset/data Job Market Dataset


Dataset name: Jobs A 2025 Dataset
Source: https://www.kaggle.com/datasets/jakupymeraj/jobs-a-2025-dataset/data
Data Author: Jakub Pymeraj
### Context: 
Explain what the dataset represents (job postings, features like salary, location, skills, etc.) and how these different features interact
### Size & Features
* 4000 rows, 20 columns
* Column entries (dtype):
    * id (int64)
    * title (object)
    * company_name (object)
    * category_label (object)
    * category_tag (object)
    * country (object)
    * location_display (object)
    * location_area (object)
    * latitude (float64)
    * longitude (float64)
    * contract_type (object)
    * contract_time (object)
    * salary_min (float64)
    * salary_max (float64)
    * salary_mid (float64)
    * salary_is_predicted (int64)
    * created_dt (datetime64[ns, UTC])
    * created_date (datetime64[ns])
    * redirect_url (object)
    * adref (object)
### Columns of interest
`category_tag`: Type of job that is listed
`country`: Country that job listing is posted (8 unique values)
`salary_min`: Minimum salary for listed job
`salary_max`: Maximum salary for listed job
`salary_mid`: Mid point between minimum and maximum salary (equal to `salary_min` if no max value)
`salary_is_predicted`: Binary value indicating if salary was predicted (1 - yes, 0 - no)
`created_date`: Date job listing was posted (YYYY-MM-DD)
### Tools and Technology
* **Python 3.x** via Anaconda
* **Jupyter Lab** for interactive development
* **Git/GitHub** for version control
* **Microsoft Copilot** for formatting, brainstorming, and plot generation
* **Key libraries:** Pandas, Matplotlib, Seaborn
### Notebooks and Data Files
* `notebooks` folder:
    * `01_data_cleaning.ipynb`: contains code that reads and cleans raw data file `dfall_clean.csv`
    * `02_data_cleaning.ipynb`: contains code and markdown that reads and analyzes cleaned DataFrame `cleaned_data.pkl` (important to run `01_data_cleaning.ipynb` before running this notebook).
* `data` folder:
    * `raw` folder:
        * `dfall_clean.csv`: raw data file downloaded from kaggle
    * `cleaned_data.pkl`: cleaned DataFrame created at the end of `01_data_cleaning.ipynb`
### Purpose of project
* Practice techniques learned in the INSY6500 course on a real world data set
* Develop questions to analyze the data applying the EDA workflow:
    1. Load and Initialize Reconnaissance
    2. Data Quality Assessment
    3. Cleaning Decisions
    4. Statistical EDA
    5. Transformation
    6. Save & Document
* Demonstrate understanding in skills and professionalism found in traditional analytic work using Python
### References
Royle, Orianna Rosa. “The September Surge: Now Is the Best Time to Find a New Job, According to the Experts.” Fortune.Com, Sept. 2023, p. N.PAG. EBSCOhost, research.ebsco.com/linkprocessor/plink?id=1b989329-32f7-3910-88d8-4869d3238d0b.
seaborn. “Seaborn: Statistical Data Visualization — Seaborn 0.9.0 Documentation.” Pydata.org, 2012, seaborn.pydata.org/.
Pandas. “Pandas Documentation — Pandas 1.0.1 Documentation.” Pandas.pydata.org, 2024, pandas.pydata.org/docs/.
Matplotlib. “Matplotlib: Python Plotting — Matplotlib 3.3.4 Documentation.” Matplotlib.org, 2024, matplotlib.org/stable/index.html.
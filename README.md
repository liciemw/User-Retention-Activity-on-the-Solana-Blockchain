# 📊 Solana Blockchain Activity & Retention Analysis 

This project analyzes **user behavior**, **developer activity**, and **program interactions** on the Solana blockchain using data queried from [Flipside Crypto](https://flipsidecrypto.xyz/).

It explores:
- New user onboarding trends
- Weekly program engagement
- Retention behavior
- Program usage patterns

---

##  Datasets Overview & Cleaning

Each dataset was cleaned to remove duplicate entries and ensure consistency across weekly and daily logs. The cleaned datasets include:

```python
df_fda_no_duplicates = df_fda_cleaned.drop_duplicates()
df_fdl_no_duplicates = df_fdl_cleaned.drop_duplicates()
df_swnu_no_duplicates = df_swnu_cleaned.drop_duplicates()
df_swnp_no_duplicates = df_swnp_cleaned.drop_duplicates()
df_slud_no_duplicates = df_slud_cleaned.drop_duplicates()
df_swup_no_duplicates = df_swup_cleaned.drop_duplicates()
df_swuu_no_duplicates = df_swuu_cleaned.drop_duplicates()

Visual Insights
Each chart is generated with Plotly and saved as a static .png. You can regenerate them in your Jupyter notebook.

1️- Weekly New Users
Visualizes how many new wallets joined the Solana blockchain each week.

2️- Weekly Unique Programs
Represents how many distinct smart contracts (programs) were executed weekly, indicating development and usage trends.

3️- Weekly Unique vs New Users
An overlay chart comparing unique active users vs newly onboarded users each week.

Bars = new users

Lines = unique active users

4️- Retention Curve
Retention Curve = % of users still active after X days.
This plot helps identify how sticky user activity is over time.

Filtered to the first 30 days after a user's first transaction.



 Setup & Environment
Ensure you have the following installed:

bash
Copy
Edit
pip install pandas plotly kaleido
Kaleido is required to save Plotly figures as .png. If you're using Anaconda:

bash
Copy
Edit
conda activate your-env
pip install kaleido
Kaleido is already satisfied if you see: Requirement already satisfied: kaleido in ...

 Project Structure
bash
Copy
Edit
├── data/                         # CSVs / processed datasets
├── weekly_new_users.png
├── weekly_unique_programs.png
├── weekly_unique_vs_new_users.png
├── number_of_days_active.png
├── U-R-A-O-S-B.ipynb    # Main analysis notebook
└── README.md
 Author
Alice M
Blockchain Research | Data Scientist 
GitHub: @liciemw

 Data Source
All insights are powered by data from [Flipside Crypto](https://flipsidecrypto.xyz/).


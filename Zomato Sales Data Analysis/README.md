## README — Zomato Restaurant Data Analysis

**Project Overview**



This project performs an exploratory data analysis (EDA) of a Zomato dataset using Python in a Jupyter Notebook environment. The goal is to uncover insights related to:



Restaurant ratings, including distribution and sentiment (via rating text/color).

Trends in cuisines and their popularity.

Country-wise and city-wise restaurant distribution.

Metrics such as online delivery prevalence.

Locations (countries/cities) with restaurants showing zero ratings.

Visual and statistical summaries of dataset structure.



**Files in the Repository**



analysis.ipynb — The main Jupyter Notebook containing code, visualizations, and analysis commentary.

zomato (1) (2).csv — Raw Zomato dataset (CSV format).

Zomato_Country-Code.xlsx — Lookup file mapping country codes to country names.

(Optional) requirements.txt — Details required Python libraries and versions.



**Setup & Dependencies**



To set up your environment, run:

pip install pandas numpy matplotlib seaborn jupyter

Then, launch and work through:

jupyter notebook analysis.ipynb



**Project Workflow & Highlights**



1. **Importing Libraries & Data**

Standard imports: pandas, numpy, matplotlib.pyplot, seaborn.

Loaded: Restaurant dataset via pd.read_csv()

Country code lookup via pd.read_excel()

2. **Initial Data Exploration**

Displayed the DataFrame, data types, and structure using df.info(), df.shape, and df.describe() (numeric and object types).

Checked for missing values using df.isnull().sum().

3. **Data Cleaning**

Filled missing values in the Cuisines column using the mode.

Merged dataset with country names using a left join on "Country Code".

4. **Descriptive Analysis & Visualizations**

Plotted:

Number of restaurants per country (scatter plot).

Distribution of ratings by count, color, and text.

Bar and count plots illustrating rating counts by color.

Pie chart of top cities by number of restaurants.

Pie charts showing most and least popular cuisines.

Created grouped DataFrames:

Ratings aggregated by rating value, text, and color.

Count of restaurants per country by the “Has Online delivery” flag.

5. **Insights & Interpretations**

Within your notebook, you might discuss findings such as:

Which countries have the most restaurants

Rating patterns and what they mean

Cities with the highest presence of Zomato-listed restaurants

Popular and underserved cuisines

Correlations (if any) between delivery options and rating distribution

Sample Visual Snippets

(Consider including completed images in the notebook or repository to help users preview your work.)

**How to Use This Notebook**



Clone or download the repository:

git clone <repo-url>
cd <repo-directory>


**Install dependencies and open the Notebook:**

pip install -r requirements.txt  

Execute cells sequentially to see the data analysis and visualizations unfold.


**What You’ll Learn**

By exploring this notebook, you’ll gain experience in:

Data cleaning and handling missing values.

Merging datasets for enriched context (country names).

Aggregating, grouping, and visualizing data using seaborn and matplotlib.

Interpreting and summarizing findings from a real-world dataset.

Developing a structured analysis workflow within Jupyter.
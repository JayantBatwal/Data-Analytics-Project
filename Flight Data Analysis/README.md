## README — Flight Data Analysis

**Project Overview**



This Jupyter Notebook explores a Flight Analysis dataset to perform data cleaning, feature engineering, and generate key insights and visualizations. It guides you through


Preparing and cleaning the dataset (handling missing values, transforming formats).

Engineering date and time features for deeper analysis.

Visualizing relationships between flight details (like stops, airlines, source) and pricing.

Drawing actionable insights such as peak booking times and revenue trends.


**File Structure**




Flight Data Analysis.ipynb — Main Jupyter Notebook with step-by-step code, comments, and visualizations.

Data_Train.xlsx — Raw input dataset containing flight details and pricing.

requirements.txt — Dependencies required to replicate analysis.

(Optional) README.md — Documentation overview (this file).


**Setup & Dependencies**



Install the required Python libraries using :

pip install -r requirements.txt

Suggested dependencies ( in a requirements.txt ):


**Workflow & Highlights**



Imports & Configuration

Libraries loaded: numpy, pandas, matplotlib, seaborn, warnings.


Dataset is imported using pd.read_excel.

Core exploratory analysis through df.info(), .shape, .describe(), and null-value checks.

Identified null entries across columns like Airline, Date_of_Journey, etc.

Imputed missing values using appropriate strategies (mostly mode or mean for ‘Price’).

Converted date/time columns (Date_of_Journey, Dep_Time, Arrival_Time) into datetime types for accurate analysis.

Transformed Total_Stops from categorical to numeric (e.g., "non-stop" → 0).


**Extracted useful features like:**



Month_of_Journey and Day_of_Journey

Dep_hour, Dep_min, Arrival_hour, Arrival_min

Removed unnecessary original columns post-extraction.

Visual Explorations

Histogram of Number of Stops vs. Flight counts.

Box plot of Flight Prices by Airline and by Source City.

Scatter visualizations for journey timing against stops.

Monthly flight counts and revenue insights via bar charts.


**Key Insights Highlighted**




Distribution of flights across different stopages.

Identification of priciest and cheapest airlines.

Source city price variability (e.g., Bangalore vs. Kolkata).

Patterns in stopages relative to journey day and month.

Top revenue-generating months.

Ideas for Extension & Enhancement

Enhance visualizations with interactivity (e.g., using Plotly).

Aggregate prices to reveal trends by route or airline.

Apply predictive modeling—like regression or classification for pricing.

Incorporate external data (seasonality, holidays) for richer insights.


**Getting Started**




Clone the repo.

Ensure dependencies are installed

Open the notebook via:

jupyter notebook Flight Data Analysis.ipynb

Walk through each section, examine the code, and explore your own visualizations.

CREATED BY - JAYANT BATWAL
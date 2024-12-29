# MTA Subway Major Incidents Analysis (2020-Present)
## Overview
This project analyzes the MTA Subway Major Incidents dataset, focusing on delays affecting 50 or more trains from 2020 to the present. By examining trends and patterns, the goal is to uncover actionable insights that could help improve subway operations and better understand the factors contributing to disruptions.

## Dataset Overview
The dataset tracks major subway incidents, categorized into the following types:

## Track: Track-related issues (e.g., fires, broken rails).
Signals: Signal failures and related issues.
Persons on Trackbed/Police/Medical: Incidents involving medical emergencies, police activity, or unauthorized persons on tracks.
Stations and Structure: Structural or power issues affecting stations or tracks.
Subway Car: Issues related to the trains themselves (e.g., door, brake, or air conditioning failures).
Other: Incidents due to external factors such as weather, vandalism, or special events.

## The dataset includes:

Time Period: From January 2020 to the present.
Key Variables:
month: Date of the incident.
division: Subway division (A or B).
line: Specific subway line affected.
day_type: Weekday (1) or Weekend (2).
category: Type of incident.
count: Number of incidents for each month/line.
Key Questions
This analysis addresses questions such as:

How do major incidents vary across different subway divisions and lines?
Which incident categories are most common?
How do weekday incidents differ from weekend incidents?
What are the peak months or lines most affected by incidents?

## Repository Structure
```plaintext
Copy code
|-- data/
|   |-- raw_data.csv           # Original dataset
|   |-- cleaned_data.csv       # Preprocessed dataset
|
|-- notebooks/
|   |-- data_analysis.ipynb    # Jupyter notebook for analysis
|
|-- visuals/
|   |-- incident_trends.png    # Key visualizations
|
|-- README.md                  # Project documentation
|-- LICENSE.md                 # Licensing information
```

How to Reproduce the Analysis
To run the analysis and generate the visualizations, follow these steps:

1. Clone the Repository
Start by cloning this repository to your local machine:

bash
Copy code
git clone https://github.com/yourusername/mta-subway-incidents.git
cd mta-subway-incidents
2. Install Dependencies
Ensure you have Python 3.7 or later installed. You can install the required dependencies using pip:

bash
Copy code
pip install -r requirements.txt
The requirements.txt file includes the following key packages:

pandas - For data manipulation.
matplotlib - For data visualization.
seaborn - For advanced visualizations.
jupyter - For running Jupyter notebooks.
3. Data Preparation
The raw dataset (data/raw_data.csv) is already included in the repository. If you wish to update the data, download the latest version from the source and place it in the data/ directory. The preprocessing script (data_analysis.ipynb) will handle cleaning and transformation.

4. Run the Analysis
Open the Jupyter notebook to perform the analysis:

bash
Copy code
jupyter notebook notebooks/data_analysis.ipynb
Follow the steps in the notebook to load the data, clean it, and generate insights.

5. Visualizations
After running the analysis, visualizations will be saved in the visuals/ directory (e.g., incident_trends.png). You can modify the analysis or add new visualizations as needed.

Data Collection
Incident data is entered manually by train dispatchers into the Integrated Train Register Activity Console (I-TRAC), which tracks delays and assigns them to specific incidents. The dataset is updated monthly, and delays are categorized based on the dispatcher’s judgment, though multiple incidents can affect the same train.

Note on Data Limitations
Data from March and April 2020 may not fully represent the usual service due to the COVID-19 pandemic and subsequent schedule changes.
Incident categories are based on dispatcher assessments and may not always reflect the exact cause of delays.
Data Dictionary
Data Label	Data Type	Description
month	DATE	The month when the incident occurred (yyyy-mm).
division	TEXT	The subway division (A or B).
line	TEXT	The specific subway line affected.
day_type	NUMERIC	1 for weekdays, 2 for weekends.
category	TEXT	The type of incident (Track, Signals, etc.).
count	NUMERIC	Number of major incidents for that month and subway line.
Release Notes
Version 1.0.0: Initial dataset release with system-wide rows removed (11/13/2024).

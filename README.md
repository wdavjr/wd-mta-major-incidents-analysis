# MTA Subway Major Incidents Analysis (2020-Present)

## About the Project
This project analyzes the **MTA Subway Major Incidents** dataset, focusing on delays affecting 50 or more trains from 2020 to the present. The goal is to uncover meaningful trends and insights that can inform operational improvements and better understand incident impacts.

## Dataset Information
The dataset includes:
- **Time Period:** January 2020 onward
- **Key Variables:**
  - `month`: Month of the incident
  - `division`: Subway division (A or B)
  - `line`: Subway line involved
  - `day_type`: Weekday (1) or Weekend (2)
  - `category`: Incident category (e.g., Track, Signals, Subway Car)
  - `count`: Number of incidents per month and subway line

## Questions Addressed
- How do major incidents vary over time and across subway divisions/lines?
- Which categories of incidents are most prevalent?
- Are there significant differences between weekday and weekend incidents?
- What months or lines are most affected?

## Repository Structure
```plaintext
|-- data/
|   |-- raw_data.csv           # Original dataset
|   |-- cleaned_data.csv       # Preprocessed data
|
|-- notebooks/
|   |-- data_analysis.ipynb    # Jupyter notebook for analysis
|
|-- visuals/
|   |-- incident_trends.png    # Key visualizations
|
|-- README.md                  # Project documentation
|-- LICENSE.md                 # Licensing information

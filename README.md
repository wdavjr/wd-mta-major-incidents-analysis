# MTA Subway Major Incidents Analysis

## Overview

This repository contains an analysis of the **MTA Subway Major Incidents** dataset, which includes data on incidents occurring within the MTA subway system starting in 2020. The data is sourced from [data.ny.gov](https://data.ny.gov/Transportation/MTA-Subway-Major-Incidents-Beginning-2020/j6d2-s8m2/about_data) and provides insights into major subway incidents across New York's metropolitan area.

## General Description

The **Metropolitan Transportation Authority (MTA)** is a public-benefit corporation responsible for managing and overseeing public transportation in New York State. It serves 12 counties in southeastern New York and two counties in southwestern Connecticut under contract with the Connecticut Department of Transportation (CDOT). The MTA operates the largest transportation network in North America, which includes a vast subway system.

This analysis aims to explore, visualize, and interpret the dataset of major subway incidents that have occurred since 2020. The dataset provides valuable information for identifying patterns, trends, and key factors that contribute to these incidents, with a focus on improving the safety and reliability of the subway system.

## Data Source

The dataset is publicly available on [data.ny.gov](https://data.ny.gov/Transportation/MTA-Subway-Major-Incidents-Beginning-2020/j6d2-s8m2/about_data) and includes the following key fields:

- **Incident Date**: The date the incident occurred.
- **Incident Location**: The location of the incident within the subway system.
- **Cause**: The cause of the incident.
- **Description**: A detailed description of the incident.
- **Impact**: The severity of the incident and its impact on service.

## Goals of the Analysis

- **Explore the dataset**: Investigate the distribution and characteristics of incidents across time, location, and cause.
- **Identify trends**: Examine patterns in the frequency and severity of incidents over time.
- **Visualization**: Create visualizations to help communicate insights from the data, including heatmaps and time-series plots.
- **Improvement suggestions**: Based on findings, suggest possible areas for improving subway system safety and incident prevention.

## Files and Structure

- `data/`: Folder containing the raw dataset and any processed files.
- `analysis/`: Folder with Jupyter notebooks or Python scripts performing the analysis.
- `visualizations/`: Folder with images or interactive plots generated during the analysis.
- `README.md`: This file.

## Requirements

To run the code and analysis in this repository, you'll need the following Python libraries:

- `pandas`
- `matplotlib`
- `seaborn`
- `plotly`
- `jupyter`

You can install the required packages by running:

```bash
pip install -r requirements.txt

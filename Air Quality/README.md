# Air Quality Data Analysis

## Overview
This repository contains an exploration of air quality data collected from an Italian city. The goal of this repository is to analyze, clean, and extract insights from the dataset using various data processing and visualization techniques.

## About the Dataset
- **Source:** [UCI Machine Learning Repository - Air Quality Dataset](https://archive.ics.uci.edu/dataset/360/air+quality)
- **Donated on:** March 22, 2016
- **Description:** This dataset contains hourly measurements of air pollutants and sensor readings collected from a gas multisensor device deployed in a polluted area at road level within an Italian city. The device recorded data from March 2004 to February 2005.
- **Characteristics:** Multivariate, Time-Series
- **Instances:** 9358
- **Features:** 15

### Dataset Information
The dataset consists of 9358 instances of hourly averaged responses from an array of 5 metal oxide chemical sensors embedded in an Air Quality Chemical Multisensor Device. Ground truth hourly averaged concentrations for CO, Non-Methanic Hydrocarbons, Benzene, Total Nitrogen Oxides (NOx), and Nitrogen Dioxide (NO2) were provided by a co-located reference certified analyzer.

### Feature Description
| Index | Feature Name | Description |
|--------|-----------------|--------------------------------------|
| 0 | Date | Date in DD/MM/YYYY format |
| 1 | Time | Time in HH.MM.SS format |
| 2 | CO (mg/m³) | True hourly averaged concentration (reference analyzer) |
| 3 | PT08.S1 (tin oxide) | Sensor response (nominally CO targeted) |
| 4 | NMHC (µg/m³) | True hourly averaged overall Non-Methanic Hydrocarbons concentration |
| 5 | Benzene (µg/m³) | True hourly averaged Benzene concentration |
| 6 | PT08.S2 (titania) | Sensor response (nominally NMHC targeted) |
| 7 | NOx (ppb) | True hourly averaged NOx concentration |
| 8 | PT08.S3 (tungsten oxide) | Sensor response (nominally NOx targeted) |
| 9 | NO2 (µg/m³) | True hourly averaged NO2 concentration |
| 10 | PT08.S4 (tungsten oxide) | Sensor response (nominally NO2 targeted) |
| 11 | PT08.S5 (indium oxide) | Sensor response (nominally O3 targeted) |
| 12 | Temperature (°C) | Ambient temperature |
| 13 | Relative Humidity (%) | Measured humidity |
| 14 | Absolute Humidity | Absolute humidity measurement |

## Repository Structure
This repository contains the following files:

- **AirQuality.csv** - The raw air quality dataset obtained from UCI.
- **cleaned_air_quality.csv** - The cleaned version of the dataset after preprocessing.
- **air_quality.ipynb** - A Jupyter Notebook containing code for data analysis and visualization.
- **requirements.txt** - Lists the dependencies required to run the analysis.
- **README.md** - Documentation of the repository.

## Notebook - air_quality.ipynb
In the `air_quality.ipynb` notebook, the dataset has been loaded and preprocessed by handling missing values and cleaning the data. Exploratory data analysis (EDA) has been performed using visualizations like histograms and correlation heatmaps to identify trends in air pollution levels. Feature engineering has been applied by creating new variables and transforming existing ones to enhance the dataset’s usability. Additionally, statistical analysis has been conducted to uncover patterns, correlations, and seasonal variations in pollutant levels. These analyses provide valuable insights into air quality trends, laying the foundation for further research and predictive modeling.

You can further analyze this dataset by applying machine learning models to gain deeper insights into air quality trends. Regression models like Linear Regression and Random Forest can help predict pollutant concentrations, while classification models such as SVM and Neural Networks can categorize air quality levels. Time series models like ARIMA and LSTMs can forecast future pollution trends, and anomaly detection techniques can identify unusual spikes, aiding in environmental monitoring and policy decisions.

## Usage Guide
### Option 1: Clone the Repository
```bash
# Clone the repository
git clone https://github.com/chitesh-marmat/Datasets-Explorations.git

# Navigate to the Air Quality directory
cd Datasets-Explorations/Air Quality

# Install dependencies
pip install -r requirements.txt
```

### Option 2: Manually Download the Cleaned Data
1. Navigate to the repository.
2. Download `cleaned_air_quality.csv` manually.
3. Use it in your analysis script or Jupyter Notebook.

### Running the Jupyter Notebook
To run the notebook, execute the following commands:
```bash
jupyter notebook air_quality.ipynb
```


 

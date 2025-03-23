# US Cities Data Analysis 
## Objective: 
### The goal of this project is to identify in what United States Citiems with populations of at least 250,000, it is most optimal to live based on cost of living, walkability, and amenities. 

## Overview:
### This analysis is designed to assist individuals when considering relocation to other cities within the United States at time of retirement. The amenities of interest include public amenities that are found in public parks, community centers, and senior centers. Of particular interest if finding cities which have low cost of living, high walkability score, and higher nubmers of amenities. 

### The project utilizes a Jupyter Notebook and python to merge two data sets. Cleaning of the data sets is accomplished via multiple steps for each data set before the merge. Teh data visualization is completed with in the Jupyther notebook as well using matplotlib. 

## Primary Files
### 1. **urban_connectivity.csv:**
### 2. **us_cities.csv:**
### 3. **Data_Dictionary.md:**
### 4. **README.md:**
### 5. **Cleaning_USCIties_Connectivity.ipynb:**
### 6. **requirements.txt:**

## Running the Program:
### The following is a guide to running the project files locally:
1. Fork the repository https://github.com/TinaBaldwin/US_Cities_Data.git
2. Clone the repository to your Github account
3. Access the repository from your command line or preferred command software (CMD).
4. Install a virtual environment. The command in Gitbash is *python -m venv venv*
5. Activate the vitual environment. The command in Gitbash is *source venv/scripts/activate*
6. Install the *requirements.txt* file to install necessary packages by running *pip install requirements.txt*



## Sources:
# Datasets (There are two data sets used and both come from Kaggle (https://www.kaggle.com/). These data sets have been cleaned and merged into one.)
-  US Cities (https://www.kaggle.com/datasets/louise2001/us-cities): For cities within the United states, this data set includes city, state, population, cost of living, etc.  
- US Cities Urban Connectivty: EDA (https://www.kaggle.com/code/vellis1/us-cities-urban-connectivity-eda): Got cities within the United States, this data set includes city, state, Walk Score and numbers of amenities like tennis courts, walking trails, basketball hoops, public restrooms, etc.

## Features:
1. Loading Data - Read in two CSV data files.
2. Data preparation - In the first three sections of Cleaning_USCities_Connectivity.ipynb the data is cleaned, merged, and new values are calculated based on the new data set.  
3. Visualization of data - The fourth section of Cleaning_USCities_Connectivity.ipynb uses Matplotlib to crease 3+ visualizations of data. 
4. Data Dictionary - Data_Dictionary.md is a custom built data dictionary document. 
5. Virtual Environment usage - Readme document includes instructions on how to setup a virtual environment. 
6. interpretation - The fifth section of Cleaning_USCities_Connectivity.ipynb contains the final analysis of the data and future recommendations.



## Directions for downloading and running the project:
# 1. clone the repository from GitHub - https://github.com/TinaBaldwin/US_Cities_Data.git
# 2. cd into the project directory
# 3. Create a virtual environment by using this in the project directory
#     - python -m venv venv
#  4. Activate the virtual environment 
#     - In windows - venv\Scripts\activate
#     - On MacOS/Linux - source venv/bin/activate
#     -In Git Bash - source venv/Scripts/activate
# The prompt should change and show the virtual envirnoment (venv)
# Install the required dependencies 
#     - pip install -r requirements.txt
#



These librabarys are needed to create graphs and plots for Matplot lib, searborn, Plotly:
pip install matplotlib
pip install plotly
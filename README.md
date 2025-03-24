# US Cities Data Analysis 
## Objective: 
### The goal of this project is to identify in what United States Citiems with populations of at least 250,000, it is most optimal to live based on cost of living, walkability, and amenities. 

## Overview:
### This analysis is designed to assist individuals when considering relocation to other cities within the United States at time of retirement. The amenities of interest include public amenities that are found in public parks, community centers, and senior centers. Of particular interest if finding cities which have low cost of living, high walkability score, and higher nubmers of amenities. 

### The project utilizes a Jupyter Notebook and python to merge two data sets. Cleaning of the data sets is accomplished via multiple steps for each data set before the merge. Teh data visualization is completed with in the Jupyther notebook as well using matplotlib. 

## Primary Files
### 1. **urban_connectivity.csv:** is one of the primary data sets used for the probject.
### 2. **us_cities.csv:** is the other primary data set used for the project. 
### 3. **Data_Dictionary.md:** is the custom data dictionary for this project. 
### 4. **README.md:** provides overview of the probject, information on running the project, sources of information, and description of project features. 
### 5. **Cleaning_USCIties_Connectivity.ipynb:** a Jupyter Notebook in which the steps for data cleaning, merging of data sets, calculation of new values, data visualization, and interpretation are located. 
### 6. **requirements.txt:** this is the file used for pip install of project requirements. 

## Running the Program:
### Check that your system meets the following requirements:
- Ensure you have Python installed. Python 3 is required. This project is written using version 3.11.9. You can download Python from https://www.python.org/downloads/.
- Ensure you have installed Git. This program is needed to clone the repository. You can download Git from https://git-scm.com/downloads.

### Follow these steps for running the project files locally:
1. Navigate in your browser to the repository at https://github.com/TinaBaldwin/US_Cities_Data.git
2. Open a terminal (command line) in your preferred software, i.e. Gitbash
3. In the terminal, navigate to the directory in which you want to clone the repository
4. In the browser, copy the URL for the repository
4. Enter into Gitbash: *git clone 'paste copied repository url'*
5. Navigate to the cloned folder from your terminal
6. In order to keep the project's dependencies isolated from your system's Python environment, create a virtual environment by entering the following into the terminal, based on your system; and install the required packages:
- On Windows: 
    1. if using command prompt:
        - enter *python -m venv venv* (creates new virtual environment named venv in your current directory)
        - to active virtual environment enter *.\venv\Scripts\activate* (your prompt should indicate you are now in venv)
    2. if using Git Bash:
        - enter *python -m venv venv* (creates new virtual environment named venv in your current directory)
        - then to activate enter *source venv/Scripts/activate* (your prompt should indicate you are now in venv)   
- On macOS and Linux: 
        - enter *python3 -m venv venv* (creates new virtual environment named venv in your current director)
        - to activate virtual environment enter *source venv/bin/activate* (your prompt should indicate you are now in venv)      
7. Once you are in the virtual environment, for all the above systems, enter into terminal *pip install -r requirements.txt*
8. Now you are ready to run the project!
    - If you have Jupyter Notebook installed, enter into terminal *jupyter notebook* and open the .ipynb file.
    - If you have Visual Studio Code (VS Code), you can open the .ipynb file in VS Code and run all the cells with the run all button at top of page or you can run each cell individually with the arrow/executve button on top left of each cell. 
8. When you are finished running the project, you can deactivate the virtual environment, by entering into the terminal *deactivate*


### The following packages will be required to run the program:
- pandas
- matplotlib
- numpy

## Sources:
# Datasets (There are two data sets used and both come from Kaggle (https://www.kaggle.com/). These data sets have been cleaned and merged into one.)
-  US Cities (https://www.kaggle.com/datasets/louise2001/us-cities): For cities within the United states, this data set includes city, state, population, cost of living, etc.  
- US Cities Urban Connectivty: EDA (https://www.kaggle.com/code/vellis1/us-cities-urban-connectivity-eda): Got cities within the United States, this data set includes city, state, Walk Score and numbers of amenities like tennis courts, walking trails, basketball hoops, public restrooms, etc.

## Features:
1. Loading Data - Read in two CSV data files.
2. Data preparation - In the first three sections of Cleaning_USCities_Connectivity.ipynb the data is cleaned, pandas merge completed, and new values are calculated based on the new data set.  
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
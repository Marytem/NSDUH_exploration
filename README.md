# NSDUH_exploration
Final project for UCU dataprocessing course

In this project dataprocessing techniques are used to work with NSDUH 2016 survey data.

Data taken from https://www.datafiles.samhsa.gov/study-dataset/national-survey-drug-use-and-health-2016-nsduh-2016-ds0001-nid17185

I generated 13 binary target variables based on specific survey questions. Each target is an indicator whether observed person is certain drug user or not. 
I predict these generated targets on two types of data - data without info about certain drug usage, and data wothout any info about any drug usage.

WORKFLOW: 

          1. observe_data.ipynb

          2. data_preparation.ipynb

          3. data_processing.ipynb

          4. final_datasets_creation.ipynb

          5. classification_visualisation.ipynb

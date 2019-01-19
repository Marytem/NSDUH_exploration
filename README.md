# NSDUH_exploration
Final project for UCU dataprocessing course

In this project dataprocessing techniques are used to work with NSDUH 2016 survey data.

Data taken from https://www.datafiles.samhsa.gov/study-dataset/national-survey-drug-use-and-health-2016-nsduh-2016-ds0001-nid17185

I generated 13 binary target variables based on specific survey questions. Each target is an indicator whether observed person is certain drug user or not. 

I predict these generated targets on two types of data - data without info about certain drug usage, and data wothout any info about any drug usage. The data is redused using Factor analysis and features were selected using Stepwise Forward Selection.

for more information see Report.pdf file.
Notebooks as they were created: 

          1. observe_data.ipynb   - a notebook with description of data, "first glance" on the dataset, its columns and values.
 
          2. data_preparation.ipynb  - deleting of useless columns, changing codes for missing values to nans, creation of binary targets for further classification. Most exhausting part of work as it involved hours of reading through 700 pages of survey documentation to understand what are the codes in columns, which prefixes in the column names are used for what, etc.

          3. data_processing.ipynb -  work performed in order to change general dataset: MV imputation, data separation according to the question-variable type
                                      work performed to *show* how(and comment why) I create smaller datasets for each type of drug. The 2 datasets (13x4 files in each) themselves are created in the next notebook:

          4. final_datasets_creation.ipynb - the code for generating final reduced datasets for each drug-type

          5. classification_visualisation.ipynb - training and testing classifiers on created datasets ^.
 

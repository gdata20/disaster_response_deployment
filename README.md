# disaster_response_deployment

# Disaster Response Pipeline Project


Introduction
The project aim is to analyze disaster data from Figure Eight to build a model for an API that classifies disaster messages.
A web app will be created for inputting a new message and get classification results in several categories.


Folders
Data
Contains the original data set
process_data.py is for preprocessing the original data for later modelling

Model
train_classier is for training the dataset and saving the model to a pickle file


App
Contain the files for creating the webapp




### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

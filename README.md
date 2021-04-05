# Disaster Response Pipeline Project
This is my project for Data Engineering section of Data Science Nano Degree from Udacity.  
It is a ETL and ML pipeline for classifying messages into multi-outputs.  
It's one of many examples where Data Science can help humans in the hour of need/crises by effectivly identifying messages that need attention.  

### Installation
1. Create a virtual environment: `python3 -m venv venv`
2. Activate environment `source venv/bin/activate` (For Ubuntu)
3. Install requirements `pip install -r requirements.txt`

### Instructions:
1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/  

### Files Description
- **data/process_data.py** : ETL pipeline for data cleaning, feature extraction, and storing data in a SQLite database.
- **models/train_classifier.py** : ML pipeline which loads data, trains a model, and pickles the trained model for later use.
- **app/run.py** : This file is used to launch the Flask web app that serves the trained model.

Really grateful to my trainers for the course and the stackoverflow community.

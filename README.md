# Disaster Response Pipeline Project
###  Introduction

In this project, I analyze disaster data from Figure Eight feature to build a model for an API that classifies disaster messages.

###  File structure
    .
    ├── app     
    │   ├── run.py                           # Flask file that runs app
    │   └── templates   
    │       ├── go.html                      # Classification result page of web app
    │       └── master.html                  # Main page of web app    
    ├── data                   
    │   ├── disaster_categories.csv          # Dataset including all the categories  
    │   ├── disaster_messages.csv            # Dataset including all the messages
    │   └── process_data.py                  # Data cleaning
    ├── models
    │   └── train_classifier.py              # Train ML model           
    └── README.md

### Instructions:

- To create a processed sqlite db
`python data/process_data.py disaster_messages.csv disaster_categories.csv DisasterResponse.db`

- To train and save a pkl model
`python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

- To deploy the application locally
`python app/run.py`

- To test app
Go to http://0.0.0.0:3001/

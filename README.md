# Pneumonia predictor
Pneumonia predictor is a end to end Flask application that predicts whether a person has pneumonia or not

##installation
one can install required packages for this application using 
```bash
pip install -r requirements
```

##usage
After installing the required packages use the following command to start the flask app
```bash
python app.py
```

##folder structure
.
├── static                            (all css and js files required will be present here) 
    ├── css                      
        └── main.css
    └── js
        └── main.js
├── templates                         all html files required willo be present here
    └── index.html
├── uploads                           when a image is tested using front end that gets stored here
├── app.py                            our application's wsgi
├── model_resnet50.h5                 our model
├── PNEUMONIA_classification.ipynb    File that developed .h5
├── Procfile                          required for deployment in heroku
├── requirements.txt                  packages required will be present here
├── training.txt                      training process
├── accuracy.png                      
└── loss.png


.
├── ...
├── docs                    # Documentation files (alternatively `doc`)
│   ├── TOC.md              # Table of contents
│   ├── faq.md              # Frequently asked questions
│   ├── misc.md             # Miscellaneous information
│   ├── usage.md            # Getting started guide
│   └── ...                 # etc.
└── ...

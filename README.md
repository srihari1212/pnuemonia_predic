# Pneumonia predictor
Pneumonia predictor is a end to end Flask application that predicts whether a person has pneumonia or not

## Dataset
Thanks to Kaggle
You can find dataset [HERE](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)

## installation
one can install required packages for this application using 
```bash
pip install -r requirements
```
## Separate environment
Alwas create a separate `conda environment/any environment` so that you can avoid version errors between packages

## usage
After installing the required packages use the following command to start the flask app
```bash
python app.py
```

## folder structure
```bash
'
.
├── static                            (all css and js files required will be present here) 
    ├── css                      
        └── main.css
    └── js
        └── main.js
├── templates                         all html files required willo be present here
    └── index.html
├── uploads                           when a image is tested using front end that gets stored here
├── app.py                            our applications wsgi
├── model_resnet50.h5                 our model
├── PNEUMONIA_classification.ipynb    File that developed .h5
├── Procfile                          required for deployment in heroku
├── requirements.txt                  packages required will be present here
├── training.txt                      training process
├── accuracy.png                      
└── loss.png
```




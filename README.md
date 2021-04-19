# Pneumonia predictor
Pneumonia predictor is a end to end Flask application that predicts `whether a person has pneumonia or not`

Created By
----------
Sri hari K V
https://bit.ly/34R7lrj

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

## About Resnet50
Resnet50 is a `pretrained model` by Imagenet which is `50 layers deep` and already got trained with 1000 categories. Here I used `transfer learning` process to retrain resnet50 for pneumonia data obtained from kaggle. 

## Important Tools used
* python 3.7
* anaconda-jupyternotebook
* conda environment
* flask
* html
* css
* js

## Training time
I trained the model through `50 epoch (cycles)`
For 50 cycles it took aroung `6 hours`

## Accuracy range
The overall accuracy range was between `88 to 91`

## Input 
After running the application just upload a `x-ray image`

## Output
It will say whether
    `The person is normal`
                or
    `The person has pnuemonia`
    
## Deployment
Now this is running `locally in my PC`
I tried with `Heroku` platform
But I couldnt deploy , since I used `Git LFS` to upload my 98.3mb .h5 model file, heroku couldnt pull LFS files to its server since I only have a `FREE TIER` account  

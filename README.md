# Age Prediction From Images
## Project description
The supermarket chain Good Seed would like to explore whether Data Science can help them adhere to alcohol laws by making sure they do not sell alcohol to people underage.  
Therefore this project should evaluate if a machine learning based system could support the cashiers or completely perform the age checks with photos from a video camera.
## Content
Within this project the following steps have been carried out: 

- Exploratory Data Analysis
- Preparing 4 Scripts to train a Deep Learning model on a computer cluster:
	- load_train  
	\-> contains a ImageDataGenerator and loads the train data
	- load_test   
	\-> contains a ImageDataGenerator and loads test and valid data
	- create_model  
	\-> contains the model architecture and building (ResNET50 backbone + custom layers)
	- train_model  
	\-> trains the built model with the given Parameters
- Evaluation of the returned model

## Outcome
- The trained Deep Learning model archives a validation and test MAE from round about at 5.87
- Based performance of the model has to be improved to be deployed because ~6 Years is an error which is too high to control legal issues
- The model could be improved using more specific user data, using a more complex structure (but carefull to not overfit) or more training epochs

# Project Name
Detect Diseases and Treatments from Sentences using NLP


## Table of Contents
* [General Info](#general-information)
* [Conclusions](#conclusions)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)

## General Information
Predict name of Diseases and Treatments from a given sentence.
Done using Custom NER (Name Entity Recognition) technique, also known as Conditional Random Field (CRF)
For Ex: 
“The patient was a 62-year-old man with squamous cell lung cancer, which was first successfully treated by a combination of radiation therapy and chemotherapy.”
A person with a non-medical background cannot understand the various medical terms. We have taken a simple sentence from a medical data set to understand the problem and where you can understand the terms ‘cancer’ and ‘chemotherapy’. 
This model is built just to do this, to predict the diseases and treatments.

- Features are defined which are required in CRF.
- Some fetures are :
    1. Whether the previous word's pos is a preposition.
    2. Whether the previous word is a NOUN and is written in Capital
    3. Whether the current word is NOUN.
    4. And so on

## Conclusions
- Using the test dataset made from features set 2, we were able to predict 98 combinations of Diseases and Treatments
  - Got the accuracy of 90.5%
- In next attempt the model was built using only those sentences which have either 'T' or 'D' label present in sentences, and this model gave accuracy of 85%, and predicted 154 combinations of Diseases and Treatments.

## Technologies Used
- sklearn-crfsuite
- Spacy
- pycrf
- Numpy
- Pandas

## Contact
Created by [@sirohijai22] - feel free to contact me!

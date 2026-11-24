# **Predicting Native VHH Aggregation**

This repository contains the models associated with the VHH aggregation paper.

To run the models, pysicochemical properties should be calculated at pH 7.4 using Molecular Operating Environment.

## **Installing Dependencies**

Both models were run in Python version 3.9. Dependencies are listed in requirements.txt.

## **Classifier Model**

Example code to run the Classifier Model can be found in the "VHH_Aggregation_classifier.ipynb" notebook in the Classifier folder. 

Note the input to the model should be a Pandas DataFrame with the following format (VHH-1 and VHH-2 shown as examples): 

|Id|app_charge|hyd_moment|
|:-: |:-:|:-:|
|VHH-1|1.77|184.9|
|VHH-2|1.92|261.6|

## **Regressor Model**
Example code to run the Regressor Model can be found in the "VHH_Aggregation_regressor.ipynb" notebook in the Regressor folder. 

Note the input to the model should be a Pandas DataFrame with the following format (VHH-1 and VHH-2 shown as examples):
|Id|pI_seq|patch_pos_n|dipole_moment|asa_hph|hyd_moment|patch_ion_1|patch_cdr_hyd|patch_cdr_ion_n|patch_hyd_n|patch_neg_n|
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|VHH-1|9.20|2.8|312.4|2461.6|184.9|50|120|2|3|0|
|VHH-2|9.28|3.0|325.8|2391.6|261.6|50|202|1|4.6|0|
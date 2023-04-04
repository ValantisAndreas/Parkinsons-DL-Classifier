# Parkinsons-DL-Classifier

## About
A  Deep Learning approach utilizing a CNN based on **Inception V3** model, for classifing fMRI scans to Parkinson Disease group or Healthy group.
This model was developed as part of a semester project in the Mobile & Electronic Health Technologies course @ NTUA 2021-2022.

## Data
For this project the database [ds000245](https://openfmri.org/dataset/ds000245/) from OpenNeuro was used.

The data were converted from the initial `.nii` format to `.png` format using the converter that can be found [here](https://github.com/alexlaurence/NIfTI-Image-Converter.git). After conerting the images to png format some data cleaning was performed and the resulting data split is the following:

|            | Healthy | PD | 
| -----------| --------| ---|
| Train      | 170     | 170|
| Validation | 34      | 34 |
| Test       | 17      | 17 |

## Score -  Confusion Matrix 

|       | Accuracy | Precision | Recall | F1   | 
| ------| ---------| ----------| -------| -----|
| Score | 64.7%    | 58.6%     | 100%   | 36.9%|

|            | Healthy | PD | 
| -----------| --------| ---|
| Healthy    | 17      | 12 |
| PD         | 0       | 5  |

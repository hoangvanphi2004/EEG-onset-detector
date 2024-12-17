<div align='center'> 
  
  # EEG onset detection    
  This repository contains experiement result of our neuroscience final project.
</div>

## Files structure

This repository contains 2 jupyter notebooks. 

+ ```eeg-cnn-gru.ipynb```: This notebook proccess the training phase. We preprocess data, train model and evaluate the model, all in this file.
+ ```eeg-demo.ipynb```: This notebook visualize the output of our model.

## Dataset
Our dataset is the CHB-MIT Scalp EEG Dataset. The dataset include recordings collected from 22 subjects (5 males, ages 3–22; and 17 females, ages 1.5–19). All signals were sampled at 256 samples per second with 16-bit resolution. Most files contain 23 channels (24 or 26 in a few cases). The International 10-20 system of EEG electrode positions and nomenclature was used for these recordings.

The `RECORDS` file contains a list of all 664 `.edf` files included in this collection, and the `RECORDS-WITH-SEIZURES` file lists the 129 of those files that contain one or more seizures. The `SUBJECT-INFO` file contains the gender and age of each subject. (Case chb24 was added to this collection in December 2010, and is not currently included in `SUBJECT-INFO`.)

In all, these records include 198 seizures (182 in the original set of 23 cases); the beginning (`[`) and end (`]`) of each seizure is annotated in the `.seizure` annotation files that accompany each of the files listed in `RECORDS-WITH-SEIZURES`. In addition, the files named `chbnn-summary.txt` contain information about the montage used for each recording, and the elapsed time in seconds from the beginning of each `.edf` file to the beginning and end of each seizure contained in it.

The original dataset source: https://physionet.org/content/chbmit/1.0.0/ 

We used the Kaggle version of the dataset, which share the same structures yet easier to import: https://www.kaggle.com/datasets/abhishekinnvonix/seizure-epilepcy-chb-mit-eeg-dataset-pediatric

## Experiment result

Our experiment result is shown below. This table show that our proposed model has outperformed other models like CNN and MLP. 

![image](https://github.com/user-attachments/assets/2873e070-da7b-4aa1-bc59-7f0a433a476b)

## Requirements
- `torch`
- `mne`

## How to use
Our project runs entirely on Jupyter Notebook using the Kaggle platform. To run the program, simply import the notebook into Kaggle and execute it.

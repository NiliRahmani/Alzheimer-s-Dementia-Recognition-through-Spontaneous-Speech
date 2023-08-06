Introduction
This repository contains code and information related to the recognition of Alzheimer's Dementia through spontaneous speech. The main idea is to extract relevant features from the speech signals and train a classification model using these features. The primary paper used for feature selection is titled "Simple and robust audio-based detection of biomarkers for Alzheimer's disease."

Feature Extraction
The code Feature_Extraction.ipynb is responsible for reading all the audio files one by one and clipping them into 20-second length segments with a 1-second overlap. After the clipping process, it extracts features from each clipped file. To enhance data diversity, the clipping and feature extraction process has been repeated for all files with four different speeds: 0.7, 0.8, 1.2, and 1.3.

Problem Formulation
The problem has been approached in two different cases:

Classification considering 2 classes (normal or with dementia).
Classification considering 4 classes, taking into account the stage of dementia (classes: normal, stage 1, stage 2, stage 3).
Model Training
The model_training.ipynb notebook is responsible for training four different models using the extracted features. The results have been presented and analyzed, showing that the RandomForest model achieved the highest accuracy. Therefore, it has been selected as the best model for prediction.

Audio Files
Please note that due to GitHub's file size limit of 100.00 MB, the audio files could not be uploaded directly to this repository. Instead, you can [access the audio files here](https://drive.google.com/drive/folders/1jNgJuWBAFtE-TMdUQ45ZFlfNT1TUkO4a?usp=sharing).


For any questions, suggestions, or collaborations, feel free to reach out.

Thank you!

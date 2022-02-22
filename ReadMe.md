Alzheimer's Dementia Recognition through Spontaneous Speech
The ADReSSo Challenge

My main idea to solve this issue is extracting some features out of the speech signals and then training a classification model using the features. The main paper that I have used for feature selection is: "Simple and robust audio-based detection of biomarkers for Alzheimer’s disease". 

The code 'Feature_Extraction.ipnb' reads all the audio files one by one, clipps them to some 20 second length files which have a overlap of 1 second. then it extracts the features out of each clipped file. For data augmentation, the clipping and feature extraction process has been repeatd for all the files with 4 new speeds: 0.7 ,0.8 , 1.2 and 1.3.

finally the 'model_training.ipnb' trains a random forest model using the extracted features and the results have been shown. 
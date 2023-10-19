Implementing a Dynamic Voting Ensemble for rumour detection

The Twitter Dataset is already in the datasets folder.
Data is already prepared for PHEME and Weibo, however if you would like to download the raw data visit the links below:  
https://figshare.com/articles/dataset/PHEME_dataset_for_Rumour_Detection_and_Veracity_Classification/6392078  
https://www.dropbox.com/s/46r50ctrfa0ur1o/rumdect.zip?dl=0  

Requires python>3.8, create the environment with requirements.txt file

Need to install the glove twitter pre-trained embeddings from https://nlp.stanford.edu/projects/glove/, then place the files in a folder named "glove".  
Create a directory named "spacy-twitter", then use the command `python -m spacy init vectors en glove\glove.twitter.27B.200d.txt spacy-twitter` to allow spacy to use the dataset.

Run model_optimizer.ipynb to get a set of optimized parameters for a confidence/size configuration

Paste those parameters into d_weight_voting.ipynb, then run the notebook with the corresponding confidence/size configuration to get results
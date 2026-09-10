# schizophrenia-detection-model
A cnn model to predict schizophrenia patients using 19 channel eeg
Each patient has 19 channels of eeg, total number of patients is 28, 14 healthy and 14 schizophrenic patients
Preprocessing and epoch extraction was done, where shizophrenia subject 10 had all epochs bad so lastly we had to drop that subject
After epoch extraction pearson correlation was done and 19*19 brain spatial connectivity matrix was obtained for each subject
then the subjects were shuffled and spilt into train test matrices and trained using a 2d cnn model
Since total dataset is small so model had a overfitting achieveing 99 percent accurcy but test evaluation was around 50 percent accuracy
which was cross checked with other models like svm, random forest and logistic regression and the accuracy hovered around 50 percent

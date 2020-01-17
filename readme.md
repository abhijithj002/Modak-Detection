STEP 1 : DATA COLLECTION
I have downloaded the Modak images from google. Also random images are downloaded not containing modak, A total of 330 images are downloded then we slpit into train (train.zip) and val folder we use 90:10 (297:33) train-test split . Both the train and val folder contains two folder modak and not_modak(two classes). 

LINK FOR DOWNLOADING TRAIN FOLDER
https://drive.google.com/file/d/1EZB19_-TYyBYhWx5LR8lxEg8fUxcXCqU/view?usp=sharing

STEP 2 : AUGMENTATION
I have augmented the data with the help of ImageDataGenerator function of keras.

STEP 3 : TRAINING
To train the network we use pre - trained VGG16. And trained for 20 Epochs and i have used batch size 2, As the ram on my system is low. We obtain accuracy of 96.9% on Validation Set.


STEP 4 : FINETUNNING
Initial training was done by freezing all the pre trained layers. Now we train all layers and use SGD optimizer instead of RMSProp .we obtain accuracy of 100% on Validation set after fine tunning.







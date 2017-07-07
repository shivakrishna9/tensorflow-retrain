# tensorflow-retrain
Using Imagenet algorithm to train your own set of images.

#Installation
Python must be installed. Install tensorflow and clone the repo.

#Get the code running
Create the  folder training_dataset .
This folder should contain the image data sets for all the subjects, for whom the classification is to be performed. 
File tree should be like..

/training_dataset
|
|
---- /larry
|    larry1.jpg
|    larry2.jpg
|    ...
|
|
---- /james
     james1.jpg
     james2.jpg

"Make sure that the number of images for each class should be atleast 30."
Run $ bash train.sh
THe script will install the Imagenet files i,e training summaries, retrained graphs and retrained labels will be saved in a folder named tf_files

Run $python classify.py image.jpg
image.jpg is the custom image to classify.
Output is the prediction accuracy.

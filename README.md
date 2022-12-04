# Animal_ID_CNN
Convolutional Neural Network: preprocessing, model analysis

The purpose of this project was to create a model that could atleast identify with 50% accuracy 10 different animals/bugs.

This project uses a dataset from kaggle.com. The dataset contains nearly 30,000 images of 10 different animals/bugs. Using this dataset my task is to work with inbalanced data since some classes have a lot more images than others. Also in order to use my model, i needed to make sure all the images were equal size. I created a function that crops images from the center and leaves a image of size 150x150. 
Next I encoded the animal/bug classes and created a training set, validation set, and test set.
Finally, I created a Convolutional neural network. Through trial and error i was able to come up with the values i used for convolution filtering and hidden layers.
After fitting the network, we can see how the model slowly starts to overfit. As the training loss goes down, the validation loss dips but then starts increasing. The classification report shows the precision, recall, F1 score and support. These values are used to judge the models performance. Lastly, I show some images at the end where the title shows the predicted image class and the real class.

Findings:
Additional preprocessing was necessary in order to get better quality images and better model performance. This is due to the fact that not all classes have similar image counts. The classes have an imbalanced amount of images. This leads to a AVG precision and recall score of 0.48. This means that half of the time the model correctly classifies an image. In order to increase this number we need more images. 

In order to increase the number of images in these classes, I used data augmentation. The Pillow library allowed me to resize all my images and I was also able to horizontally flip images in certain classes that needed it. These two simple lines of code were able to replace a function i had created to resize images by cropping. 

Using this new model defintely seems promesing for me. I hope i can break the 48% precision and recall and go past 50%. Running only 4 epochs does not show the whole story but i achieved 62% AVG precision and recall. With more time set aside this model can be left to train for a couple hours for a proper evaluation.

Some of the things i tried and were not shown is hyper parameter tuning. Parameters like size of neural network and size of convolutional filters were attempted but they took too long and i preferred a quicker trial and error method. 

Also in my first version of my code i had a function that resized all my images into a size of 150x150. It did this though croping from the center. Using this function lead to large images appearing zoomed in. This pre-processing method that i used was too destructive on the data. Instead i used Tensorflows resize function.

Another feature i wanted to implement but took up too much ram was normalizing the images.

Overall this project was a great experience, the only parts that i did not like was waiting for the model to train. Each epoch was about 20 minutes so for this final version i only ran it for 4 epochs but i was planning to do around 15.

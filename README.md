# Animal_ID_CNN
The purpose of this project was to create a model that could atleast identify with 50% accuracy 10 different animals/bugs

This project uses a dataset from kaggle.com. The dataset contains nearly 30,000 images of 10 different animals/bugs. Using this dataset my task is to work with inbalanced data since some classes have a lot more images than others. Also in order to use my model, i needed to make sure all the images were equal size. I created a function that crops images from the center and leaves a image of size 150x150. 
Next I encoded the target classes and created a training set, validation set, and test set.
Finally, I created a Convolutional neural network. Through trial and error i was able to come up with the values i used for convolution filtering and hidden layers.
After fitting the network, we can see how the model slowly starts to overfit. As the training loss goes down, the validation loss starts increasing. The classification report shows how well the model performed.
Lastly, I show some images at the end where the title shows the predicted image class and the real class.

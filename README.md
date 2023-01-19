### Animal_ID_CNN
**Isaac Rodriguez-Jimenez**

#### Executive Summary

#### Rationale
Now a days, phones and cameras have machine learning algorythms built into them. On some phones, when you take a picture of an animal, sometimes it will be able to tell you what kind of animal it is. This problem is called image classification. This type of machine learning model not only applies to animals but to everything else in the world than can be named/classified. These models have the potential to indentify any object so it is best to understand its fundamentals with pictures of animals.

#### Research Question
My initial question was to find out if i could create a model that could at the very minimum achieve 50% accuracy readings.

#### Data Sources
The data i used was a collection of folders that included pictures of animals. These pictures were all of different sizes and resolutions. They were downloaded from Kaggle.com and included 10 different animals with a minimum of 1000 pictures per folder. https://www.kaggle.com/datasets/alessiocorrado99/animals10

#### Methodology
-Initial image manipulation required resizing of all images to a standardized size i chose of 150x150x3. 
-Due to imbalances in the animal image count. I decided to transpose images in order to flip them and add them to thier folders. This was done to increase image count for certain animals.
-After creating the convolutional model. I ran some metrics testing in order to determine how my model performed.

#### Results
My initial results on my first version gave me an average precision and recall of 0.48.
In my second version i achieved an average precision and recall of 0.62 just by changing the way my images were being saved and increasing the testing set.

#### Outline of project

- [Link to notebook 1]()
- [Technical Write Up](https://github.com/0IsaacR/Animal_ID_CNN/blob/main/Technical%20Finding)
- [Link to notebook 3]()


##### Contact and Further Information
https://www.linkedin.com/in/risaac13/

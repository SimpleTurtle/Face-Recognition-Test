# Face-Recognition-Test
### Training a face recognizer using OpenCV

This face recognition program is based on the tutorial found [here](https://www.superdatascience.com/opencv-face-recognition/). I attempted to create a facial recognition program that would be able to differentiate between several subjects. I used the LBP face cascade to get the training done more quickly, but I do plan on letting it run with haar for more accurate predictions. For my subjects, I chose to use several members of the K-Pop group Dreamcatcher, as K-Pop idols have a large amount of fan pictures that are able to be used to train the program. I tried to have the program train on pictures from every member of the group, but I ran into memory issues that prevented me from doing so. This program doesn't seem to work as well I would have hoped, as the program seems to think that the members look similar and confuses them quite often. 

Another problem I ran into was that opencv's face detection algorithms don't work perfectly. It detects some pictures as containing no faces even though the main focus of the image is the idol's face. This leads to instances where it trains to recognize a patch of foliage in the picture as the idol's face instead of the idol's actual face. Example image below. I wonder how it might perform if it were to be trained on people from a different ethnic background. 

![Sample text](https://github.com/SimpleTurtle/SimpleTurtle/blob/master/images/22344172_1300303463430014_37224820856848384_n.jpg)

I added successful prediction pictures to show what the face recognition program is able to do when it runs correctly. These are available to view [here](predictions/).

Some data:

2,310 pictures were used in total to train the program
* 645 pictures of Jiu
* 564 pictures of Handong
* 551 pictures of Gahyeon
* 550 pictures of Yoohyeon

1,799 faces were detected in the 2,310 pictures, although each picture contained a face

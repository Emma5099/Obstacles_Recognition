# Obstacles Recognition
## Detects with two methods (image processing and neural network), the shape and color of an obstacle.

This project is a part of a bigger project: the command of a robot (with Stm32, Raspberry, communication master-slave)for it to move in space, switch on the light, capture sound, diffuse sound...)
A part of the project was to take pictures of obstacles, to tell what type of obstacles they were and to avoid them.
I had the idea of detecting the shapes and colors with image recognition. 
I then introduce a dataset of pictures of the differents obstacles to 'train' the algorithm. 

I did my own dataset by random pictures of the obsctacles around.

The result works ok but could be way better if the dataset was larger. The dataset was stocked locally in this computer so  it was impossible to input a larg set of datas.
Especially for pictures from the side, it is difficult for the program to detect what shape it is. 
But the most important: as the shapes are really simples, increasing the convolution layers does not improve the accuracy of the model. The best way can be to do simple image processing on the imafe (as I did with the Image_test code)
 
There is two codes: 
- the Image_Test.py (that is just image processing to detect shapes and color)
- the Image_Real.py (that is a AI that understand the shapes)


This program has been inspired from a youtube video: https://www.youtube.com/watch?v=6FHtTyZxS5s
I did not took car of the limits of the embedded system (storage, speed, CPU...)

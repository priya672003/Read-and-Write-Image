## EX.NO :01

## DATE : 

# <p align="center"> READ AND WRITE AN IMAGE </p>

## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.


## Program:


## Developed By: PRIYADARSHINI R
## Register Number :  212220230038
```python


# To Read,display the image

import cv2
color_image = cv2.imread("photo.jpg",1)
cv2.imshow('212220230038 , PRIYADARSHINI',color_image)
cv2.waitKey(0)


# To write the image

import cv2
color_image = cv2.imread('photo.jpg',1)
w = cv2.imwrite('img.png',color_image)
cv2.imshow('212220230038 , PRIYADARSHINI',color_image)
cv2.waitKey(0)


# Find the shape of the Image

import cv2
import random
color_image = cv2.imread('photo.jpg',1)
print(color_image.shape)


# To access rows and columns

import cv2
import random
color_image = cv2.imread('photo.jpg',1)
for i in range(100):
    for j in range(color_image.shape[1]):
        color_image[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
    
cv2.imshow('212220230038 PRIYADARSHINI',color_image)
cv2.waitKey(0)


# To cut and paste portion of image

import cv2
color_image = cv2.imread('photo.jpg',-1)
tag = color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212220230038',color_image)
cv2.waitKey(0)








```
## Output:

### i) Read and display the image

![OUTPUT 1](https://user-images.githubusercontent.com/81132849/161373328-3cf00dce-1d77-4887-baff-5581ed998b40.png)

### ii)Write the image

![OUTPUT 2](https://user-images.githubusercontent.com/81132849/161373450-ac2844b4-2ccf-46b5-b232-5ab5ff211387.png)

### iii)Shape of the Image

![OUTPUT 3](https://user-images.githubusercontent.com/81132849/161373462-ca79f599-f330-4891-b519-986f729fe940.png)

### iv)Access rows and columns

![OUTPUT 4](https://user-images.githubusercontent.com/81132849/161373486-3eaf74f5-81df-4834-9cd7-4868372f3f20.png)

### v)Cut and paste portion of image

![OUTPUT 5](https://user-images.githubusercontent.com/81132849/161373506-21cfa7cc-6004-4253-8339-9e8f9ea60d1e.png)



## Result:
Thus the images are read, displayed, and written successfully using the python program.



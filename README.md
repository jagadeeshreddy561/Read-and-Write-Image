# READ AND WRITE AN IMAGE
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
### Developed By:
### Register Number: 
i) #To Read,display the image
```python
  import cv2
image1=cv2.imread('nature.jpg',1)
cv2.imshow('212222240059',image1)
cv2.waitKey(0)
cv2.destroyAllWindows

```
ii) #To write the image
```python

import cv2
image1=cv2.imread('nature.jpg',1)
cv2.imwrite("nature.jpg",image1)
cv2.imshow('212222240059',image1)
cv2.waitKey(0)

```
iii) #Find the shape of the Image
```python
import cv2
pic = cv2.imread("nature.jpg",1)
print(pic.shape)


```
iv) #To access rows and columns

```python
import random
import cv2
pic=cv2.imread("nature.jpg",1)
for i in range(100):
    for j in range(pic.shape[1]):
        pic[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("212222240059",pic)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```python

import cv2
capture=cv2.imread("nature.jpg",1)
tag=capture[260:280,100:300]
capture[60:80,100:300]=tag
cv2.imshow("212222240059",capture)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

![OUTPUT](/Screenshot%20from%202023-03-15%2011-22-27.png)

### ii)Write the image
![OUTPUT](/2.png)
<br>
<br>

### iii)Shape of the Image
![OUTPUT](/3.png)

<br>
<br>

### iv)Access rows and columns

![OUTPUT](/4.png)
<br>

### v)Cut and paste portion of image
![OUTPUT](/5.png)
## Result:
Thus the images are read, displayed, and written successfully using the python program.



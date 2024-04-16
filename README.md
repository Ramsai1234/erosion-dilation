# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary pacakages


### Step2:
Create the text using cv2.putText

### Step3:
Create the structuring element

### Step4:
Erode the image

### Step5:
Dilate the Image

 
## Program:
```
Developed by : P Ramsai
Reg No:212221240041

```
## Import the necessary packages
```
import cv2
import numpy as np
from matplotlib import pyplot as plt
```


# Create the Text using cv2.putText
```
img1 = np.zeros((100, 400), dtype='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'sai ram',(5,70),font,2,(255),5,cv2.LINE_AA)

```


# Create the structuring element
```
kernel = np.ones((5,5), np.uint8)
kernel1 =  cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_erode1 = cv2.erode(img1,kernel1)
image_dilatel = cv2.dilate(img1,kernel1)
print(image_erode1)
print(image_dilatel)
plt.imshow(img1)
plt.axis("off")
```


# Erode the image
```
plt.imshow(image_erode1)

```



# Dilate the image
```
plt.imshow(image_dilatel)


```
## Output:

### Display the input Image:
![image](https://github.com/Ramsai1234/erosion-dilation/assets/94269989/911cbd2b-2851-4d37-83b0-d3c944bb8809)



### Display the Eroded Image:

![image](https://github.com/Ramsai1234/erosion-dilation/assets/94269989/5b64a88c-2532-4221-8796-19f0a0c6202e)


### Display the Dilated Image:
![image](https://github.com/Ramsai1234/erosion-dilation/assets/94269989/14660fce-2533-4ae7-8809-3289a1482602)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.

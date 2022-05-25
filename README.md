# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.
 
## Program:
```
/*
Developed by   : Kumaran B
Register Number: 212220230026
*/
```
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((300,500),dtype='uint8')
font=cv2.FONT_ITALIC=3
img2=cv2.putText(img1,"Kumaran",(5,70),font,3,(255),5,cv2.LINE_AA)
cv2.imshow("Original",img2)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Create the structuring element
kernel1=np.ones((5,5),np.uint8)

# Erode the image
erode=cv2.erode(img2,kernel1)
cv2.imshow("Erosion1",erode)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Dilate the image
dilute=cv2.dilate(img2,kernel2)
cv2.imshow("Dilution",dilute)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### Display the input Image
![Screenshot (260)](https://user-images.githubusercontent.com/75243072/170279130-3604073d-e5df-422d-9cb3-f9b9230e00e6.png)

### <br><br>Display the Eroded Image
![Screenshot (261)](https://user-images.githubusercontent.com/75243072/170279169-17d70edf-5dc5-4b2c-85cd-fab558905e70.png)

### Display the Dilated Image
![Screenshot (262)](https://user-images.githubusercontent.com/75243072/170279233-cdd4c1f9-3239-4fb3-81aa-75319d30a8f4.png)

## <br><br><br><br><br><br><br><br>Result
Thus the generated text image is eroded and dilated using python and OpenCV.

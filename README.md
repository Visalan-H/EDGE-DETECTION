# EDGE-DETECTION
## Aim:
To perform edge detection using Sobel, Laplacian, and Canny edge detectors.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import all the necessary modules for the program.

### Step2:
Load a image using imread() from cv2 module.

### Step3:
Convert the image to grayscale

### Step4:
Using Sobel operator from cv2,detect the edges of the image.

### Step5:

Using Laplacian operator from cv2,detect the edges of the image and Using Canny operator from cv2,detect the edges of the image.

## Program:
##### Developed By: Visalan H
##### Register Number: 212223240183
<br>

#### Original Image:
```
import numpy as np
import cv2
import matplotlib.pyplot as plt

input_img = cv2.imread("ex6.jpg")
input_img = cv2.cvtColor(input_img, cv2.COLOR_BGR2RGB)

plt.axis('off')
plt.imshow(input_img)
plt.title("Original Image")
plt.show()
```

### Sobel Edge Detector:
<br>

#### Sobel X:
```
sobelx = cv2.Sobel(gray,cv2.CV_64F,1,0,ksize=5)
plt.imshow(sobelx,cmap='gray')
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```

#### Sobel Y:
```
sobely = cv2.Sobel(gray,cv2.CV_64F,0,1,ksize=5)
plt.imshow(sobely,cmap='gray')
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```

#### Sobel XY;
```
sobelxy = cv2.Sobel(gray,cv2.CV_64F,1,1,ksize=5)
plt.imshow(sobelxy,cmap='gray')
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```

### LAPLACIAN EDGE DETECTOR:
```
lap=cv2.Laplacian(gray,cv2.CV_64F)
plt.imshow(lap,cmap='gray')
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```


### CANNY EDGE DETECTOR
```
canny=cv2.Canny(gray,120,150)
plt.imshow(canny,cmap='gray')
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```
## Output:

### SOBEL EDGE DETECTOR

![image](https://github.com/user-attachments/assets/d36a70c5-1181-4248-a797-96ecf4f486df)


### LAPLACIAN EDGE DETECTOR

![image](https://github.com/user-attachments/assets/e925b619-3a62-452d-9998-7ccbf9214ce2)


### CANNY EDGE DETECTOR

![image](https://github.com/user-attachments/assets/aaf92db9-a058-40ef-bad7-f222b428237c)

## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.

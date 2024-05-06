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
## Developed by:VISHAL M.A
## Register Number: 212222230177

```p
import cv2
import matplotlib.pyplot as plt

image=cv2.imread('flower.jpg',0)
```
```p
gray_image=cv2.cvtColor(image,cv2.COLOR_GRAY2RGB)
gray_image=cv2.GaussianBlur(gray_image,(3,3),0)
```
## Sobel X Axis
```p
sobelx=cv2.Sobel(gray_image,cv2.CV_64F,1,0,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray_image)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelx)
plt.title("Sobel X axis")
plt.axis("off")
plt.show()
```
## Sobel Y Axis
```p
sobely=cv2.Sobel(gray_image,cv2.CV_64F,0,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray_image)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobely)
plt.title("Sobel Y axis")
plt.axis("off")
plt.show()
```
## Sobel XY Axis
```p
sobelxy=cv2.Sobel(gray_image,cv2.CV_64F,1,1,ksize=5)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray_image)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(sobelxy)
plt.title("Sobel XY axis")
plt.axis("off")
plt.show()
```
## LaplacianEdge Detector
```p
lap=cv2.Laplacian(gray_image,cv2.CV_64F)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray_image)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(lap)
plt.title("Laplacian Edge Detector")
plt.axis("off")
plt.show()
```
## Canny Edge Detector
```p
canny=cv2.Canny(gray_image,120,150)
plt.figure(figsize=(8,8))
plt.subplot(1,2,1)
plt.imshow(gray_image)
plt.title("Original Image")
plt.axis("off")
plt.subplot(1,2,2)
plt.imshow(canny)
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```
## Output:
### SOBEL EDGE DETECTOR
## Sobel X Axis
![og img 1](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/60979217-4dd7-4348-ab02-e63d17462713)
![sobel x](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/68436dd6-612e-4d38-863b-e11fad7a54c0)

## Sobel Y Axis
![og img 2](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/aeac4436-b9b9-4a76-b8cb-64883dfaeb5b)
![sobel y](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/a585c48d-047e-4c03-8d0d-afc2d301503a)


## Sobel XY Axis
![og img 3](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/311b1538-1e29-41b3-a841-75801ffa63d5)
![sobel xy](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/6e75f2ea-7760-4cb9-94f5-e5c9b3876f4f)



### LAPLACIAN EDGE DETECTOR
![og img 4](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/9871ef94-298e-4c51-85fa-cc5c83376423)
![lap img](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/c8b1369a-20b6-4d82-9a21-a48fa7e6863d)




### CANNY EDGE DETECTOR
![og img 5](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/103a6d25-2f45-42b5-a138-00fb1361ccdf)
![canny edge](https://github.com/vishal21004/EDGE-DETECTION/assets/119560110/3d441e4a-18bd-43d8-b456-724430e41123)



## Result:
Thus the edges are detected using Sobel, Laplacian, and Canny edge detectors.

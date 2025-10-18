# THRESHOLDING
## Aim
To segment the image using global thresholding, adaptive thresholding and Otsu's thresholding using python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm

### Step1:
Load the necessary packages.
### Step2:
Read the Image and convert to grayscale.
### Step3:
Use Global thresholding to segment the image.

### Step4:
Use Adaptive thresholding to segment the image
### Step5:
Use Otsu's method to segment the image and display the results
## Program


# Load the necessary packages
```
import cv2
import numpy as np
import matplotlib.pyplot as plt

```





# Read the Image and convert to grayscale
```
# Step 2: Read the image and convert to grayscale
image = cv2.imread(r'C:\Users\admin\Desktop\DIPT\DIPT SAI IMG.jpg')  # Replace with your image file path
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)  # Convert to grayscale

```




# Use Global thresholding to segment the image
```
plt.subplot(2, 2, 2)
plt.imshow(global_thresholded, cmap='gray')
plt.title("Global Thresholding")
plt.axis('off')

```




# Use Adaptive thresholding to segment the image
```
plt.subplot(2, 2, 3)
plt.imshow(adaptive_thresholded, cmap='gray')
plt.title("Adaptive Thresholding")
plt.axis('off')
```



# Use Otsu's method to segment the image 
```
plt.subplot(2, 2, 4)
plt.imshow(otsu_thresholded, cmap='gray')
plt.title("Otsu's Method")
plt.axis('off')
```



# Display the results
```
plt.tight_layout()
plt.show()
```





## Output

### Original Image
<img width="209" height="311" alt="image" src="https://github.com/user-attachments/assets/5e6234d4-de25-4c9d-a473-3ea435393538" />


### Global Thresholding
<img width="256" height="324" alt="image" src="https://github.com/user-attachments/assets/dcb81b7e-a995-40bd-91dc-d7c9e7a42344" />


### Adaptive Thresholding
<img width="297" height="341" alt="image" src="https://github.com/user-attachments/assets/da1ab383-9cf7-4ca8-9da8-fc1e9538f1db" />


### Optimum Global Thesholding using Otsu's Method
<img width="246" height="337" alt="image" src="https://github.com/user-attachments/assets/e08c3bed-13d4-45dd-b5a0-096d07358a6a" />



## Result
Thus the images are segmented using global thresholding, adaptive thresholding and optimum global thresholding using python and OpenCV.

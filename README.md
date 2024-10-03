# THRESHOLDING
## Aim
To segment the image using global thresholding, adaptive thresholding and Otsu's thresholding using python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm

### Step1:
Load the input image using cv2.imread() and convert it to a grayscale image using cv2.cvtColor() with the color conversion code cv2.COLOR_BGR2GRAY.

### Step2:
Use a fixed threshold value (e.g., 127) for global thresholding with cv2.threshold(). Pixels with intensity above this value are set to maximum intensity (255), and the rest are set to minimum intensity (0).

### Step3:
Use adaptive thresholding, which calculates the threshold for smaller regions of the image. The threshold is calculated dynamically using cv2.adaptiveThreshold() with the ADAPTIVE_THRESH_GAUSSIAN_C method.

### Step4:
Otsu's method automatically finds an optimal threshold value by minimizing the within-class variance. Apply it using cv2.threshold() with the flag cv2.THRESH_OTSU.

### Step5:
Use plt.imshow() to visualize the grayscale image and the segmented images from global, adaptive, and Otsu's thresholding techniques.
## Output

### Original Image

![img](https://raw.githubusercontent.com/Girithickrohan/Thresholdingg/refs/heads/main/Screenshot%202024-10-03%20162622.png)

### Global Thresholding

![img](https://raw.githubusercontent.com/Girithickrohan/Thresholdingg/refs/heads/main/Screenshot%202024-10-03%20162632.png)

### Adaptive Thresholding

![img](https://raw.githubusercontent.com/Girithickrohan/Thresholdingg/refs/heads/main/Screenshot%202024-10-03%20162643.png)

### Optimum Global Thesholding using Otsu's Method

![img](https://raw.githubusercontent.com/Girithickrohan/Thresholdingg/refs/heads/main/Screenshot%202024-10-03%20162653.png)

## Result
Thus the images are segmented using global thresholding, adaptive thresholding and optimum global thresholding using python and OpenCV.

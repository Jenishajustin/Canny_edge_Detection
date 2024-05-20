# Canny Edge Detection
## AIM
To perform edge detection using Canny edge detector.
## SOFTWARE REQUIRED
Anaconda - Python 3.7
## ALGORITHM
1. Import all the necessary modules for the program.
2. Load a image using imread() from cv2 module.
3. Convert the image to grayscale.
4. Using Canny operator from cv2,detect the edges of the image.
5. Display the result.
## PROGRAM
```
Developed By : J.JENISHA
Reg. No. : 212222230056
```
```python
import cv2
img=cv2.imread('flower.jpg')
gray=cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imwrite('flower.jpg',gray)
plt.imshow(gray,cmap='gray')
plt.title("Original gray Image")
plt.axis("off")
plt.show()

canny=cv2.Canny(gray,120,150)
plt.imshow(canny,cmap='gray')
plt.title("Canny Edge Detector")
plt.axis("off")
plt.show()
```

## OUTPUT
![Screenshot 2024-05-20 194641](https://github.com/Jenishajustin/Canny_edge_Detection/assets/119405070/c87691d8-33f5-4259-bd76-89ab601d1dc1)

![Screenshot 2024-05-20 194712](https://github.com/Jenishajustin/Canny_edge_Detection/assets/119405070/438fa2c4-07a6-4bb2-ac8b-78ac7de417d5)

## RESULT
Thus the edges are detected successfully using Canny edge detectors.

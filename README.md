# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
```
Step1:
Import necessary packages

Step2:
Create an empty window and add text to it

Step3:
create a structuring element

Step4:
Do the operation

Step5:
Show the output image
```

 
## Program:

```
NAME:KATHIRVEL.A
REG NO:212221230047

```
# Import the necessary packages
```
import cv2
import numpy as np
```


# Create the Text using cv2.putText
```
font=cv2.FONT_HERSHEY_PLAIN
cv2.putText(img1,'KATHIRVEL',(5,35),font,2,(255),5,cv2.LINE_AA)
cv2.imshow("KATHIRVEL",img1)
cv2.waitKey()
cv2.destroyAllwindows()
```

# Create the structuring element
```
kernal=np.ones((5,5),np.uint8)

```


# Use Opening operation

```
mg1o=cv2.morphologyEx(img1,cv2.MORPH_OPEN,kernal)
cv2.imshow("KATHIRVEL"img1)
cv2.waitKey(0)
cv2.destroyAllwindows()
```


# Use Closing Operation
```
imglc=cv2.morphologyEx(img1,cv2.MORPH_CLOSE,kernal)
cv2.imshow("KATHIRVEL",imglc)
cv2.waitKey(0)
cv2.destroyAllwindows()



```
## Output:

### Display the input Image



![Screenshot_20231107_132842](https://github.com/KathirvelAIDS/OPENING--CLOSING/assets/94911373/76ba9016-9919-431a-91c3-632d98ebe60b)







### Display the result of Opening


![Screenshot_20231107_132852](https://github.com/KathirvelAIDS/OPENING--CLOSING/assets/94911373/dd8dad54-ef23-4d5a-93b4-68ad80522dc0)



### Display the result of Closing


![Screenshot_20231107_132906](https://github.com/KathirvelAIDS/OPENING--CLOSING/assets/94911373/4cfedf6d-7e1e-4c07-9ee9-c23a4cd909d0)





## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.

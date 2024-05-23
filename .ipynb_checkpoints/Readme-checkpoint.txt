Collecting and labeling images using OpenCV and Labelme Library

This model can be used for any type of OBJECT DETECTION Model

PROCESS:

1. Take images from Webcam
2. Bounding box Anootation using LABELME
3. We will do data agumentation to generate more data from current data
4. Train DL model: a classification model and a regression model to draw bounding box arround object
5. Loss: 
For Classification model : Binary cross entropy loss
For regression model: Localization loss
Sum of (x-x')2 + (y-y')2   +   sum of (w-w')2 + (h-h')2

6. VGG16 model as classificaton model

output: 5 outputs
[0 or 1 ] : weather face is detected
[x1,y1, x2,y2]

Albumentation us used for data augmentation
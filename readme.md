## NQueen Problem
This code helps you to understand and draw boundaries on objects of a particular image.


### Code Requirements
The example code is in Python ([version 2.7](https://www.python.org/download/releases/2.7/) or higher will work). 

### Description

Here is the approach that I used to detect the blocks:

1.Converted the image to grayscale	
2.Applied threshold (simple binary threshold, with a handpicked value of 150 as the threshold value)
3.Applied dilation to thicken lines in image, leading to more compact objects and less white space fragments. Used a high value for number of iterations, so dilation is very heavy (13 iterations, also handpicked for optimal results).
4.Identified contours of objects in resulted image using opencv findContours function.
Drew a bounding box (rectangle) circumscribing each contoured object - each of them frames a  block of text.


For more information, [see](http://opencv-python-tutroals.readthedocs.io/en/latest/)

### Input

<img src="https://github.com/akshaybahadur21/ImageSegmentation/blob/master/input.jpg">

### Output

<img src="https://github.com/akshaybahadur21/ImageSegmentation/blob/master/output.png">



### Execution
To run the code, type `python First.py`

```
python First.py
```

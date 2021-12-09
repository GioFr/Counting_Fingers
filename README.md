# Counting Fingers using Convex Hull

In this notebook we are using Convex Hull algorithm from OpenCv to count fingers. 
This is a capstone project of the udemy course developed by Jose Portilla.

First of all we choose the region of interest which will be used as a background and where the hand will be positioned. We threshold it so we can grab a foreground. Afterwards when the hand is positioned in the roi, we segment it using convex hull, after which we find the maximum euclidean distance between the center of the palm and the most extreme points of the convex hull, later it will be used to create a circle with 80% radius of the max euclidean distance between center point and outermost points. It looks something like the following

 

<img src='images/1.png' width='180'> <img src='images/2.png' width='180'> <img src='images/3.png' width='180'> <img src='images/4.png' width='180'> <img src='images/5.png' width='180'>


 


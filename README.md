# Perspective Transformation using Line Detector and Optimization

[Thien Do-Tieu](https://github.com/dotieuthien)

### Overview
This is the Python implementation of [paper](https://www.semanticscholar.org/paper/Rectification-of-planar-targets-using-line-segments-An-Koo/e1feceb12777c06727da3b281d2b8d7472182444) 

```
https://link.springer.com/article/10.1007/s00138-016-0807-1
An, J., Koo, H.I. & Cho, N.I.
Rectification of planar targets using line segments
Machine Vision and Applications 28, 91–100 (2017).
https://doi.org/10.1007/s00138-016-0807-1
```
for perspective transformation. By using line detector, this approach creates a loss function which contains information
of tilt angle of vertical and horizontal lines, and an optimization algorithm tries to minimize loss value, simultaneously 
update rotate angles in perspective matrix. In this implementation, I used Gradient Descent instead of Levenberg–Marquardt algorithm

### Installation
Install line detector package for python 3
```
pip install pylsd
pip install ocrd-fork-pylsd
```

### Result
#### Image after rendering

<img width="1000" alt="First result" src="./img/perspective_test.png">

#### The result after cropping

<img alt="First result" src="./img/result.png">

### Reference
[Rectification of planar targets using line segments](https://www.semanticscholar.org/paper/Rectification-of-planar-targets-using-line-segments-An-Koo/e1feceb12777c06727da3b281d2b8d7472182444)

[Perspective transform opencv](https://www.pyimagesearch.com/2014/08/25/4-point-opencv-getperspective-transform-example/)

# Lane Detection
Most lanes are designed to be relatively straightforward not only as to encourage orderliness but also to make it easier for human drivers to steer vehicles with consistent speed. Therefore, our intuitive approach may be to first detect prominent straight lines in the camera feed through edge detection and feature extraction techniques. I have used OpenCV, an open source library of computer vision algorithms, for implementation. \
##  Setting up your environment
If you do not already have OpenCV installed, open Terminal and run:
```
pip install opencv-python
```


## Processing a video
We will feed in our sample video for lane detection as a series of continuous frames (images) by intervals of 10 milliseconds. We can also quit the program anytime by pressing the ‘q’ key.

## Applying Canny Detector
The Canny Detector is a multi-stage algorithm optimized for fast real-time edge detection. The fundamental goal of the algorithm is to detect sharp changes in luminosity (large gradients), such as a shift from white to black, and defines them as edges, given a set of thresholds. The Canny algorithm has four main stages:

# Understanding Computer Vision using Naive Techniques
This repository contains 5 folders with Jupyter notebooks that explore various computer vision techniques including transformations, convolution, video segmentation, and texture classification - as well as the data files used within them.

## 1. Image Transformation
I explored image transformations such as rotation and skewing. I developed a function that takes an input image, rotates it by an angle, and horizontally skews it by an angle. I also wrote a matrix formulation for image rotation skewing.

To demonstrate these transformations, I created an image that contains my name written in Arial, point 72, capital letters. I then rotated the image clockwise by 30, 60, 120, and -50 degrees and skewed it by 10, 40, and 60 degrees. 

# 2. Image Convolution
I explored convolution and its applications in image filtering. I build a function that takes an input image, performs convolution with a given kernel, and returns the resulting image. 
I also designed a convolution kernel that computes, for each pixel, the average intensity value in a 3x3 region and save the resulting image.

I then applied some kernels to the filtering function and saved the resulting images.

# 3. Video Segmentation
I explored video segmentation using colour histograms and histogram intersections. I built a histogram function that returns the colour histogram of an input image and visualises the histogram, saving the corresponding figure. For a given video sequence, I used the histogram function to construct the histogram of each frame.
I then wrote a function that returns the value of the intersection of a pair of histograms. I used the histogram intersection function to calculate the intersection between consecutive frames of a video and find how to normalize the intersection. I plot the intersection values over time and the normalized intersection values and save the corresponding figures.

I also discuss what the intersection value represents for a given input video, whether we can use it to make a decision about scene changes, how robust the histogram intersection is to changes in the video, and when it fails.

# 4. Texture Classification
I explored texture classification using the Local Binary Pattern (LBP) operator. I built a function that divides a grayscale image into equally sized non-overlapping windows and returns the feature descriptor for each window as a distribution of LBP codes. I also developed a descriptor that represents the whole image as consisting of multiple windows and implement a classification process that separates the images in the dataset into two categories: face images and non-face images.

I commented on the results and discuss whether the global descriptor is able to represent whole images of different types. I identified problems, discuss them, and suggest possible solutions. I then decreased the window size and perform classification again, followed by increasing the window size and performing classification again. 

# 5. Object Counting
I explored object detection via fixed cameras by building a function for frame referencing. I then explore counting objects using that function and attempt to visualise the counted objects.

I then commented on the implementation of my function and its advantages and disadvantages.

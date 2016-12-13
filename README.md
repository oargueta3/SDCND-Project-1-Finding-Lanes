# **Project 1: Finding Lane Lines on the Road**   
#### Udacity's Self-Driving Car Nanodegree

### Objective
When we drive, the lines on the road are the visual reference we use to steer vehicles on roads and highways. For a self-driving cars being able to make use of this reference is an important tool to navigate our current road infractructure. The objective of this project was to explore a simple methods to detect lane lines using Computer Vision techniques with Python and a dedicated library called OpenCV (Open-Computer Vision). The algorithm used and the results will be discussed in the sections below.

### Algorithm Overview
A pipeline was developed to process single images and overlay the detected lane lines. This pipeline was then applied to a video stream, which is only a collection of images. The foundation of this algorithm rest on the ability to detect edges on an image, in other words, extract just the outlines of the different contents in an image.
<img src="laneLines_thirdPass.jpg" width="480" alt="Combined Image" />

In the figure above you are able to see edges of the lane markings on the road, but you are also able to see the edes of
###### Algorithm to find lane lines on images:
1. Change image to gray scale
2. Apply Gaussian Blur to reduce image noise
3. Apply Canny Edge Detection
4. Mask the resulting image to only include the region of interest
5. Apply Hough Transform to extract Hough lines
6. Draw extrapolated lines to extend over the detected lane markings

### Results

### Useful References

### Enviroment Setup
Choose the appropriate Python 3 Anaconda install package for your operating system <A HREF="https://www.continuum.io/downloads" target="_blank">here</A>.   Download and install the package.

If you already have Anaconda for Python 2 installed, you can create a separate environment for Python 3 and all the appropriate dependencies with the following command:

`>  conda create --name=yourNewEnvironment python=3 anaconda`

`>  source activate yourNewEnvironment`

**Step 2:** Installing OpenCV

Once you have Anaconda installed, first double check you are in your Python 3 environment:

`>python`    
`Python 3.5.2 |Anaconda 4.1.1 (x86_64)| (default, Jul  2 2016, 17:52:12)`  
`[GCC 4.2.1 Compatible Apple LLVM 4.2 (clang-425.0.28)] on darwin`  
`Type "help", "copyright", "credits" or "license" for more information.`  
`>>>`   
(Ctrl-d to exit Python)

run the following commands at the terminal prompt to get OpenCV:

`> pip install pillow`  
`> conda install -c https://conda.anaconda.org/menpo opencv3`

then to test if OpenCV is installed correctly:

`> python`  
`>>> import cv2`  
`>>>`  
(Ctrl-d to exit Python)

**Step 3:** Installing moviepy  

We recommend the "moviepy" package for processing video in this project (though you're welcome to use other packages if you prefer).  

To install moviepy run:

`>pip install moviepy`  

and check that the install worked:

`>python`  
`>>>import moviepy`  
`>>>`  
(Ctrl-d to exit Python)

**Step 4:** Opening the code in a Jupyter Notebook

You will complete this project in a Jupyter notebook.  If you are unfamiliar with Jupyter Notebooks, check out <A HREF="https://www.packtpub.com/books/content/basics-jupyter-notebook-and-python" target="_blank">Cyrille Rossant's Basics of Jupyter Notebook and Python</A> to get started.



`> jupyter notebook`
```sh
$ cd docs
$ install -d
$ conda
```

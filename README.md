# CS 3793 Final Project

Source: https://automaticaddison.com/the-ultimate-guide-to-real-time-lane-detection-using-opencv/#Detect_Lane_Lines_in_a_Video

This is an implementation of real-time lane detection using OpenCV computer vision library and Python.


## Requirements

You must have Python 3.7 or higher to use this repo.

### Installation
Lets make sure OpenCV is installed on your machine. I will be using [pip](https://pip.pypa.io/en/stable/installation/) to install these packages. In your terminal, type:

`pip install opencv-python`

NumPy also needs to be installed:

`pip install numpy`

As well as Matplotlib:

`pip install matplotlib`

## Usage

With the provided code and files, run this command in the directory that contains all the files:

`python lane.py`

If set up correctly, a new window with this image should appear:

![enter image description here](https://raw.githubusercontent.com/jvliov/jvliov.github.io/main/original_w_lane.jpeg)

To use any other image, make sure it is in the same directory as `lane.py`. You also need to change the following line of code: 

`filename = 'YOUR_IMAGE_NAME.jpeg'`

You should also specify the four corners of the trapeziod region of interest. This is done by altering the following lines: 

	self.roi_points = np.float32([

		(343,253), # Top-left corner

		(110, 478), # Bottom-left corner

		(560,479), # Bottom-right corner

		(464,253) # Top-right corner

	])


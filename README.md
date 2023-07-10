# Disparity-Prediction

The disparity_estimation.py code implements a disparity estimation pipeline using a convolutional neural network (CNN) in Pytorch. The pipeline takes pairs of left and right stereo images as input and produces a disparity map as output.

The code defines an encoder function that creates a CNN encoder module. The encoder is used to extract image features from the input images. The code also defines a disparity estimation function that creates a convolutional layer responsible for estimating the disparity between the left and right images. The code includes a compute_cost_volume function that computes the cost volume, which is a volume that contains matching costs between image patches in the left and right images.
The disparity_net function combines the encoder, cost volume computation, and disparity estimation steps to create a complete network for estimating the disparity map. The depth_estimation function takes the estimated disparity map, baseline distance, and focal length as input and calculates the depth map. 



The disparity_estimation_1.py code is performing stereo matching using the StereoBM(Block Matching) algorithm to compute the disparity map between a pair of left and right images with the OpenCV library in Python.
Parameters for the stereo-matching algorithm include the number of disparities, block size, speckle range, speckle window size, and minimum disparity should be altered by trial and error to get the desired output.



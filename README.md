# Visual Odometry
Visual Odometry  is a crucial  concept in Robotics Perception for estimating  the  trajectory  of the robot (the camera on the robot to be precise).  The concepts involved in Visual Odometry are quite the same for SLAM which needless to say is an integral part of Perception.

In this project we are given frames of a driving sequence taken by a camera in a car,  and the scripts to extract the intrinsic parameters.  We will implement the different steps to estimate the 3D motion of thecamera, and provide as output a plot of the trajectory of the camera.

## DataSet Download
The dataset can be downloaded from here : 
https://drive.google.com/open?id=14Wxvr-pg9soeCyU0z0-CqdqsU5Q_O9kw

Place the `detectbuoy.avi` in the same folder as the code.

## How to run code
1. Unzip the folder which has the code, input sequences and the datasets.
2. Copy the Stereo images to its folder in `Oxford_Dataset/Stereo/`
3. Run data_preparation.py inside the `Oxford_Dataset` folder
4. Each of the following code parts needs to be separately run.
5. To compute fundamental matrix instead of using inbuilt RANSAC we resorted to customized RANSAC for better results but the computing was considerably slowed down. We have used both the code for comparison.
6. For Visual Odometry proposed pipeline run 
        `python3 Visual_Odometry.py`      
7. For Comparison with inbuilt OpenCV functions run 
        `python3 verification.py`

## Results
https://drive.google.com/open?id=12Wfx0IMpCe19iwCPdsoLlI3x8J590kgm

  <p align="center">
  <img src="https://github.com/ramaprashanth/visual-odometry/blob/master/result_1.png">
  </p>

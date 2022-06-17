# <Head_Pose_Estimation>

## Description
In this project, we will predict 3 angles (pitch, yaw and roll) of the head pose using 3 different models
We will use AFLW2000 dataset with contains 2000 image and 2000 matlab file with contains the 3 labels (angels).
We will use mediapipe package to extract points of the face in each image.
Trying different models for each angle and select the best one.
Applying our models to predict the 3 angles of frames of videos.

## Output Of Tested Example
![head](3CQsnT_ad6337d97eaa56bd6410aa9153e82318_00-00-00_00-00-11_2.gif)

## Notebook Steps:
-Installing Mediapipe Package
-Downloading Data & Extracting Files
-Preprocessing On Data
-Splitting data for training and validation.
-Applying Gridsearch
-Applying and Comparing Between Different Models
-Final Modeleling.
-Testing Model On Images.
-Testing Model On Videos.

# Head Pose Estimation


## Project Description

![2d-3d-head-pose-estimation](https://user-images.githubusercontent.com/49573699/191772281-32883606-2c1c-4f8e-bc9b-a56a7465cde5.jpg)

- In this project, we will predict 3 angles (pitch, yaw and roll) of the head pose using 3 different models.
- We will use AFLW2000 dataset with contains 2000 image and 2000 matlab file which contains the 3 labels (angels).
- We will use mediapipe package to extract points of the face in each image.

## Dataset
- In this project, we used AFLW2000 dataset that you can download from this [link](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/Database/AFLW2000-3D.zip). which contains 2000 image and 2000 matlab file which contains the 3 labels (angels).

## Notebook Steps:
- Installing Mediapipe Package
- Downloading Data & Extracting Files
- Preprocessing On Data
- Splitting Data For Training & Validation.
- Applying Gridsearch
- Applying and Comparing Between Different Models
- Final Modeleling.
- Testing Model On Images.
- Testing Model On Videos.

## Project Toolbox
- Mediapipe
- Sklearn
- OpenCV
- Globe
- Numpy
- Pandas

## Modeling
- Trying different models for each angle, applying Gridsearch, and select the best Model,which was `Support Vector Regressor (SVR) Model`, then Applying our 3 models to predict the 3 angles of frames of videos.

## Model Evaluation
- Metric used: `Root Mean Square Error (MAE)` and `Mean Aboslute Error (MAE)` .
For our 3 models MAE was as following:
- Yaw Angle Model:
  - RMSE: `0.19865662883247995`
  - MAE: `0.0677858562161892`

- Pitch Angle Model:
  - RMSE: `0.4875773800317196`
  - MAE: `0.09436501409366947`
  
- Roll Angle Model:
  - RMSE: `0.528458780620693`
  - MAE: `0.0677858562161892`

## Output Of Tested Example
![head](test_video.gif)




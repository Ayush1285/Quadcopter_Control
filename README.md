# Quadcopter_Control

## Introduction
  In this project,we will learn the dynamics of the Quadcopter and implement control algorithms on it.

## Altitude control of a 1D Quadcopter
### Hover at height 1 m

![](https://github.com/Ayush1285/Quadcopter_Control/blob/main/1-D_Control/Results/heightcontrol.gif)

## 2D trajectory tracking using PID controller
Goal was to track the given two dimensional trajectories while minimising the position error.
### Line Trajectory

![](https://github.com/Ayush1285/Quadcopter_Control/blob/main/2-D_Control/Results/trajline.gif)

### Sine Trajectory

![](https://github.com/Ayush1285/Quadcopter_Control/blob/main/2-D_Control/Results/trajsine.gif)

### Diamond Trajectory

![](https://github.com/Ayush1285/Quadcopter_Control/blob/main/2-D_Control/Results/trajdiamond.gif)

## 3D trajectory tracking using PID controller
Goal was to track the given three dimensional trajectories while minimising the position error.
### Helix Trajectory

![](https://github.com/Ayush1285/Quadcopter_Control/blob/main/3-D_Control/Results/trajhelix.gif)

### Minimum Snap Trajectory through given waypoints

![](https://github.com/Ayush1285/Quadcopter_Control/blob/main/3-D_Control/Results/trajminsnap.gif)

## Graphs
### Minimum Snap Trajectory following using PID
<img src="Simulink_Models/Results/xpositionpid.jpg" heigth="10"> | <img src="Simulink_Models/Results/ypositionpid.jpg">
--------------------------------------------------------|-----------------------
<img src="Simulink_Models/Results/zpositionpid.jpg">  | 

### Minimum Snap Trajectory following using LQR
<img src="Simulink_Models/Results/xpositionlqr.jpg" heigth="10"> | <img src="Simulink_Models/Results/ypositionlqr.jpg">
--------------------------------------------------------|-----------------------
<img src="Simulink_Models/Results/zpositionlqr.jpg">  | 

### Comparison of Trajectory tracking error (LQR vs PID)
<img src="Simulink_Models/Results/xposerror.jpg" heigth="10"> | <img src="Simulink_Models/Results/yposerror.jpg">
--------------------------------------------------------|-----------------------
<img src="Simulink_Models/Results/zposerror.jpg">  | 

## Simulink modelling of the Quadcopter
  * Dynamics Study of the Quadcopter according to the paper [Modelling and Stabilizing Control laws design based on Backstepping for an UAV type Quadrotor](https://drive.google.com/file/d/1x7zfYDEAd4OGHKVt8xIQ0uwxMXA-TSl7/view?usp=sharing)
  * Linearized the equations around hovering point.
  * Developed the simulink model of Quadcopter.[[Simulink Model](https://github.com/Ayush1285/Robust_Quadcopter_Control/blob/main/Simulink%20Models/Quadrotor_linearized.slx)]
  
## PID on the Quadcopter model
  Our goal was to implement PID and LQR controller on the Simulink model of Quadcopter and compare them
  
  **Minimum Snap trajectory following(Desired Path: Yellow, Obtained Output: Blue)**
  ![](https://github.com/Ayush1285/Robust_Quadcopter_Control/blob/main/Simulink%20Models/Results/PID.png)
  
## Linear Quadratic Regulator(LQR) on the Quadcopter

  **Minimum Snap trajectory following(Desired Path: Yellow, Obtained Output: Blue)**
  ![](https://github.com/Ayush1285/Robust_Quadcopter_Control/blob/main/Simulink%20Models/Results/LQR.png)
  
## Comparison of PID and LQR control system on the Quadcopter
  Here, we will compare error during the trajectory tracking
  
  **Error Plots(LQR: Yellow, PID: Blue)**
  ![](https://github.com/Ayush1285/Robust_Quadcopter_Control/blob/main/Simulink%20Models/Results/LQR%20vs%20PID.png)
  

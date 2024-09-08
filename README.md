# Ever-V-Autonomous-Track
As the Autonomous Team Leader at the Shoubra Racing Team, I had the privilege of leading my team in the prestigious autonomous EVER V Competition, which included both simulation and real-world demonstrations. 
Our efforts in the simulation competition earned us the 1st place in technical performance and 3rd place overall.
In the real demo, we secured an impressive 2nd place overall.

### My Team

<p align="center">
  <img src="https://github.com/user-attachments/assets/dfe43854-4209-4f7e-8e87-e057c191dafc" alt="Picture3" width="300" display="flex"/>
  <img src="https://github.com/user-attachments/assets/bfacdccf-0dc7-47d6-ad95-32700072b769" alt="Picture3" width="415" display="flex"/>
</p>


# Simulation Competition 1st technical 3rd overall

![455833478_829934979326065_6699800269364222313_n](https://github.com/user-attachments/assets/d6857687-a95c-477d-9087-be4c96f0863f)

# The competition was divided into three key milestones:
All the given environment is designed by us.

## Milestone 1: Open Loop Control
### In this milestone, the objective was to maneuver the car through open-loop tracks, including:
  - Straight Line
  - Straight Line with Lane Change
  - Circular Track
  - Infinity Shape Track
### Tools Used:
  - ROS1
  - CoppeliaSim
  - Algorithm: The vehicle was moved based on timed intervals, utilizing a Python timer to control the sequence of movements.
<p align="center">
  <img src="https://github.com/user-attachments/assets/ecf9dbce-6cd9-41f4-8d9e-e99f2afe487c" alt="Description">
</p>


## Milestone 2: Closed Loop Control & Object Detection
This milestone comprised two main tasks:

### Task 1: 
Implement a closed-loop controller to navigate the car, leveraging odometry feedback for precise movement. To simulate real-world conditions, Gaussian noise was added to the odometry data, making the system more realistic. The readings were then refined and stabilized using a Kalman filter algorithm, enhancing the overall accuracy and reliability of the car's navigation.
- Gaussian Noise established from Matlab.
- Kalman Filter.
<p align="center">
  <img src="https://github.com/user-attachments/assets/61535a55-c94a-49ac-8755-ba86168e83ac" alt="Description">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/59bc54f0-915a-4ccc-8f5e-70f204ea716a" alt="Description">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/c2a1951f-c1e3-46ca-9080-d78c3c67dab4" alt="Description">
</p>

### Task 2: 
Perform object detection within the simulation environment. This involved detecting both static and dynamic objects such as humans, cars, and cones. We achieved this by training a YOLOv7 model and quantizing it for efficient, real-time object detection using ONNX.

<p align="center">
  <img src="https://github.com/user-attachments/assets/941307ad-5054-482e-a782-3ca840631a1b" alt="Description">
</p>

## Milestone 3: Advanced Computer Vision and Adaptive Cruise Control
In the final milestone, the focus was on:

Implementing computer vision capabilities to detect humans and trigger emergency braking.
Detecting obstacles on the road and changing lanes when possible.
Using LIDAR sensors for adaptive cruise control, allowing the car to match the speed of the vehicle ahead.

<p align="center">
  <img src="https://github.com/user-attachments/assets/6ba06264-cc61-4070-976c-a89d222fffbf" alt="Description">
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/238dd880-6c18-46ba-90eb-a92447b97ee9" alt="Description">
</p>

# Real-World Demo Competition 2nd place
The real-world demo involved navigating the car in an infinity-shaped track using a closed-loop controller.
Implementation:
Using Pure Pursuit Algorithm and Tuned the look-ahead distance to guide the car accurately through the designated waypoints to make the car moves in infinity shape, ensuring smooth and controlled movement.

<p align="center">
  <img src="https://github.com/user-attachments/assets/ef4ac955-68d5-44a5-a0a0-70189a8bd39d" alt="Description">
  <img src="https://github.com/user-attachments/assets/141ee098-44c4-4c42-9e25-9ed85cb44960" alt="Description">
</p>

# ROS2 Differential Robot Simulation

This repository contains the ROS2 simulation of a differential drive robot using the Gazebo simulator. The robot is equipped with various sensors and utilizes SLAM and Nav2 for mapping, localization, and navigation.

## Project Overview

### Components

- **Simulation Environment:** Gazebo
- **Robot Description:** Defined using Xacro files
- **Sensors:**
  - 2D LIDAR
  - Camera
  - Depth Camera
- **Mapping and Localization:** SLAM (Simultaneous Localization and Mapping)
- **Navigation:** Nav2 (Navigation 2)

### Robot Description

The differential robot is designed using Xacro files which define the robot's physical parameters, sensor placements, and joint configurations. The robot includes the following sensors:

- **2D LIDAR:** Used for distance measurement and obstacle detection.
- **Camera:** Provides visual input from the robot's perspective.
- **Depth Camera:** Captures depth information of the environment to assist in navigation and obstacle avoidance.

### Functionalities

1. **Mapping and Localization:**
   - Utilizes SLAM to create a map of the environment in Gazebo.
   - Continuously updates the robot's position and orientation within the map.

2. **Navigation:**
   - Uses Nav2 to plan and execute paths within the mapped environment.
   - Capable of autonomous navigation to specified goals while avoiding obstacles.

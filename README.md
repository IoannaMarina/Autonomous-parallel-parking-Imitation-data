# Autonomous-parallel-parking-Imitation-data


This repository contains a dataset of state-action pairs for 20 parallel parking scenarios generated using the CARLA Simulator.

## Dataset Description

- **Actions**: The actions consist of:
  - **Steering Values**: A continuous range between -1 and 1.
  - **Reverse Flag**: A boolean indicating reverse (true for reverse, false for not reverse).

- **State**: The state files include readings from 10 radar sensors positioned primarily on the right-hand side of the vehicle, along with the following 8 spatial characteristics:
  - **Z**: The vertical position of the ego vehicle in 3-dimensional space. Determines whether the ego vehicle is positioned on the sidewalk.
  - **Angle**: The current orientation of the ego vehicle. Determines the ego vehicle’s heading.
  - **Angle Difference**: Angular variance between the current and desired orientation for parallel parking. Quantifies the deviation between the ego vehicle’s yaw and the target yaw of the parking space.
  - **Distance**: Linear proximity measurement between the ego vehicle and the target parking location. Quantifies the physical closeness of the ego vehicle to the parking space.
  - **Position**: Binary representation of the relative position of the ego vehicle. A value of 1 denotes the ego vehicle in front of the parking spot, and -1 indicates it is positioned behind. Determines whether the ego vehicle is situated in front or behind the parking space.
  - **Orientation**: Binary representation of the ego vehicle’s directional alignment. A value of 1 signifies the ego vehicle facing to the right, and -1 indicates it is oriented to the left. Determines whether the ego vehicle is facing to the left or right concerning the target orientation.
  - **Parallel Distance**: The distance between the ego vehicle and the parking space, considering parallel alignment. Measures how closely the ego vehicle aligns parallel to the parking space.
  - **Vertical Distance**: The distance between the ego vehicle and the parking space, considering vertical alignment. Measures how closely the ego vehicle aligns vertically to the parking space.

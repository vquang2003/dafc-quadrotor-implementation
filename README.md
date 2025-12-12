# UAV Trajectory Tracking Control using Simulink

## Overview
This project focuses on designing and implementing a control system for a Quadrotor UAV to follow a circular trajectory. The project demonstrates the bridge between mathematical modeling in **Simulink** and real-world experimental validation.

## Key Features
- **Mathematical Modeling:** Full dynamic model of a Quadrotor.
- **Control Algorithm:** Direct Adpative Fuzzy Controller for altitude and position tracking.
- **Real-time Implementation:** Testing the algorithm in a laboratory environment.

## Control Architecture
This image shows the block diagram of Quadrotor control system in Simulink:
<img width="1611" height="760" alt="Screenshot 2025-12-13 004837" src="https://github.com/user-attachments/assets/ce6c168a-62e8-4e13-b694-ff148c359acc" />

## Simulation Results
The performance of the controller in the Simulink environment shows perfect tracking under ideal conditions:
<img width="700" height="525" alt="untitled" src="https://github.com/user-attachments/assets/9e12cc32-40f6-4039-bcec-27f4a145013f" />

## Experimental Video
The following video shows the UAV performing a circular path in the lab. While there are some oscillations due to sensor noise and aerodynamics, the UAV successfully maintains the target trajectory.

[Click here to watch the flight test video](https://youtu.be/FhYS1LfzKBE)

The graph shows the Quadrotor's desired and actual trajectory:
<img width="700" height="525" alt="real" src="https://github.com/user-attachments/assets/b06c0f72-1b4a-4550-8dcf-ec6c185a9958" />


## Discussion
- **Simulation:** Shows near perfect tracking with zero steady-state error.
- **Experiment:** The UAV follows the circle but exhibits small oscillations. This is primarily caused by sensor noise and unmodeled aerodynamics effects, which were not present in the ideal Simulink simulation.
- **Future Work:** Improve the controller with a Kalman Filter to reduce noise.

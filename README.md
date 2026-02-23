# obstacle-aware-ros2-bot

This project features a fully modeled mobile robot equipped with ultrasonic (Sonar) and visual (Camera) sensors, designed to navigate and detect obstacles within a simulated Gazebo environment.

##  Overview
The goal of this project was to bridge the gap between robot hardware description and simulated intelligence. Using **ROS 2 Humble**, I developed a mobile robot capable of "seeing" its surroundings, which is the first step toward full autonomy and path planning.



##  Key Features
* **Custom URDF Modeling:** A detailed 4-wheeled robot chassis with defined inertial, collision, and visual properties.
* **Dual-Sensor Integration:**
    * **Sonar (Ray Sensor):** Mimics ultrasonic behavior for precise distance measurement to obstacles.
    * **Camera Plugin:** Provides real-time visual data streaming from the robot's perspective.
* **ROS 2 Architecture:** Implements standard ROS 2 messaging for sensor data and motion control.
* **Planar Move Plugin:** Enables smooth locomotion and steering control within the physics engine.

##  Tech Stack & Tools
* **Middleware:** ROS 2 (Humble Hawksbill)
* **Simulation:** Gazebo (Ignition/Classic)
* **Robot Modeling:** URDF (XML)
* **Visualization:** RViz2
* **Language:** Python / C++ (Plugin configuration)

##  Workspace Structure
```bash
dev_ws/
└── src/
    └── obstacle_aware_robot/
        ├── description/      # URDF and Xacro files
        ├── launch/           # Launch files for Gazebo/RViz
        ├── worlds/           # Custom Gazebo environment
        └── config/           # Sensor and controller parameters

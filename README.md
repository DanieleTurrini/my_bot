# Robotic Walker Project

## Overview
This project was developed as part of the **Robotic Perception and Action** course. The primary goal was to design and implement a mobile robotics simulation environment using **ROS2** and **Gazebo**. The simulation involves controlling a **deambulator** to follow a predefined path while visualizing its environment.

## Key Features
- **Path Following**: The walker autonomously follows a given trajectory.
- **Dynamic Updates**: The path and map can be updated dynamically, ensuring real-time adaptability.
- **Integration with Other Projects**:
  - A **height map generator** that constructs an environmental map using depth camera images.
  - A **path planning module** that computes an optimal route using the **potential fields algorithm**.

## Technologies Used
- **ROS2**: For robot control and simulation.
- **Gazebo**: For 3D simulation and environment rendering.
- **Depth Camera**: For environmental mapping.
- **Potential Fields Algorithm**: For path optimization.

## Getting Started
### Prerequisites
- Install **ROS2** (Humble or later recommended)
- Install **Gazebo**
- Ensure dependencies for depth camera and path planning are met

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/your-repository.git
   ```
2. Navigate to the project directory:
   ```bash
   cd my_bot
   ```
3. Build the ROS2 workspace:
   ```bash
   colcon build
   ```
4. Source the workspace:
   ```bash
   source install/setup.bash
   ```

### Running the Simulation
To launch the simulation, run:
```bash
ros2 launch my_bot simulation.launch.py
```

To make the robot move, run:
```bash
ros2 run my_bot path_follow
```


# Unified Robot Description FIle Example

URDF, Unified Robot Description Format is an XML format for representing a robot model. It is commonly used in Robot Operating System (ROS) tools such as rviz (Ros Visualization tool) and Gazebo simulator. The model consists of links and joints motion.

### demo image
<p align="center">
  <img src="https://res.cloudinary.com/diekemzs9/image/upload/v1736180017/Screenshot_from_2025-01-06_18-50-22_kow97l.png" alt="Image 1" width="615">
</p>

This repo contains an example of a URDF file and a launch script to run it. (ROS 2)


## How To Run

1. Clone this repo into your ROS2 workspace, specifically into the workspace's SRC folder  
2. setup your ros environment
3. Build the package with colcon.
4. Launch the `robot_state_publisher` launch file with `ros2 launch urdf_example rsp.launch.py`.
5. Launch `joint_state_publisher_gui` with `ros2 run joint_state_publisher_gui joint_state_publisher_gui`. You may need to install it if you don't have it already.
6. Launch RViz with `rviz2 -d <path_to_your_rviz_file>/robotview.rviz` - remember to make sure its located in your ros workspace


- Set your fixed frame to `world`
- Add a `RobotModel` display, with the topic set to `/robot_description`, and alpha set to 0.8
- Add a `TF` display with names enabled.

#### contact me ibz.04dev@gmail.com in case you run into any problem

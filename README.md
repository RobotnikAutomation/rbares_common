# rbares_common

Common packages of the Rb Ares robot: URDF description of the autonomous pallet truck, control algorithms, platform messages and other files for simulation.

## Installation

Install external dependencies:

- [joint_read_command_controller](https://github.com/RobotnikAutomation/joint_read_command_controller) : git clone https://github.com/RobotnikAutomation/joint_read_command_controller

- [robotnik_sensors](https://github.com/RobotnikAutomation/robotnik_sensors) : git clone -b melodic-devel https://github.com/RobotnikAutomation/robotnik_sensors

Also you need to install dependencies, you need to execute:

```bash
sudo dpkg -i binaries/ros-melodic-robotnik-msgs_1.1.0-0bionic_amd64.deb
```
```bash
sudo dpkg -i binaries/ros-melodic-rcomponent_1.1.0-0bionic_amd64.deb 
```
```bash
sudo dpkg -i binaries/ros-melodic-rbares-controller_0.0.0-0bionic_amd64.deb 
```
```bash
sudo dpkg -i binaries/ros-melodic-robotnik-navigation-msgs_0.0.0-0bionic_amd64.deb 
```
```bash
sudo dpkg -i binaries/ros-melodic-robotnik-move_1.0.0-0bionic_amd64.deb 
```
```bash
sudo dpkg -i binaries/ros-melodic-robotnik-docker_1.0.0-0bionic_amd64.deb  
```
```bash
sudo dpkg -i binaries/ros-melodic-rbares-elevator-controller_0.0.0-0bionic_amd64.deb
```

## Packages

### rbares_description

The urdf, meshes, and other elements needed in the description are contained here. The standard camera configurations have been included (w/wo sphere_camera, w/wo axis_camera, etc.). The package includes also some launch files to publish the robot state and to test the urdf files in rviz.

### rbares_control

This package contains the launch and configuration files to spawn the robot controllers with the ROS controller_manager. 

### rbares_navigation

This package contains the configuration for running the Navigation stack of the Rb Ares robot (ROS Navigation, Robotnik Navigation, etc) (Read rbares_navigation/README.md)

### rbares_localization

This package contains the configuration for running AMCL and map_server.

### rbares_perception

This package contains the launch files and configuration for running locator node.

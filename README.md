# rbares_common

Common packages of the Rb Ares robot: URDF description of the autonomous pallet truck, control algorithms, platform messages and other files for simulation.

## Installation

Install external dependencies:

- [joint_read_command_controller](https://github.com/RobotnikAutomation/joint_read_command_controller) : git clone https://github.com/RobotnikAutomation/joint_read_command_controller

- [robotnik_sensors](https://github.com/RobotnikAutomation/robotnik_sensors) : git clone -b melodic-master https://github.com/RobotnikAutomation/robotnik_sensors

Also you need to install binaries, you need to execute:

```bash
cd binaries
./install.sh
```

## Packages

### rbares_description

The urdf, meshes, and other elements needed in the description are contained here. The package includes also some launch files to publish the robot state and to test the urdf files in rviz.

### rbares_control

This package contains the launch and configuration files to spawn the robot controllers with the ROS controller_manager.

### rbares_navigation

This package contains the configuration for running the Navigation stack of the Rb Ares (ROS Navigation, Robotnik Navigation, etc)

### rbares_localization

This package contains the configuration for running AMCL, ICP, map_server and map_saver.


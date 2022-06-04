# Map My World Project (SLAM)

## Overview

THis project aims to perform SLAM on a robot housed in a Gazebo world using rtabmap_ros package.

**Keywords:** slam, rtab-slam, 

Or, add some keywords to the Bitbucket or GitHub repository.

**Author: Rutvik Patel<br />**

The my_robot package has been tested under [ROS] Kinetic on respectively Ubuntu 16.04.7 LTS (Xenial Xerus).
This is research code, expect that it won't be maintained for future ROS versions.




## Installation, Building and Running

### ROS Version

The project has been developed and tested on Ubuntu 16.04 LTS with [ROS Kinetic](wiki.ros.org/kinetic/).

### Dependencies

- Install [rtabmap_ros](http://wiki.ros.org/rtabmap_ros) package using the command <code>sudo apt install ros-kinetic-rtabmap-ros</code>

### Building
Use <code>catkin_make</code> to build the packages from source and source the workspace using <code>source devel/setup.bash</code> to add the files to path.

### Launching the Project
Run the following commands in separate terminals:
- Launch the world in Gazebo: <code>roslaunch my_robot world.launch</code>
- Launch the teleop node for keyboard control: <code>roslaunch my_robot teleop.launch</code>
- Launch the RTAB-Map mapping node: <code>roslaunch my_robot mapping.launch</code>

### Viewing the Result
View the map using the command: <code>rtabmap-databaseViewer ~/.ros/rtabmap.db</code> <br>
If you used a custom file path use that in the above command.
<br>
[ROS]: wiki.ros.org/kinetic/
[rviz]: http://wiki.ros.org/rviz
[rtabmap_ros]: https://github.com/introlab/rtabmap_ros
# Current Control Demo:
source /opt/ros/humble/setup.bash

cd lunabotics_ros2_ws/

source install/setup.bash

## For Starting Up Nodes:

ros2 run control_pkg testcontrol.py

ros2 run control_pkg drivetrain

ros2 run control_pkg scoop


## Notice
Do NOT colcon build yet, still working on the sparkcan packages. Instead, run:

colcon build --packages-select interfaces_pkg
colcon build --packages-select control_pkg

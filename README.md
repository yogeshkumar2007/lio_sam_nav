# LIO-SAM Navigation Workspace

This ROS 2 workspace combines Livox MID360 LiDAR support, LIO-SAM odometry and
mapping, Nav2 path planning and control, rover robot descriptions, custom
interfaces, GTSAM, and spatio-temporal voxel costmap support for autonomous
navigation.

Build outputs and runtime logs are excluded from Git. The source tree contains
the LIO-SAM package, Livox ROS 2 driver and SDK, Nav2, rover model and
navigation packages, custom interfaces, GTSAM, and the voxel layer.

## Running

```bash
ros2 launch livox_ros_driver2 msg_MID360_launch.py
ros2 launch lio_sam run.launch.py
ros2 launch rover_navigation navigation.launch.py
```
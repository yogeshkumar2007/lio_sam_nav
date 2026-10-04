# LIO-SAM Navigation

This ROS 2 workspace combines Livox MID360 LiDAR support, LIO-SAM odometry and
mapping, Nav2 path planning and control, rover robot descriptions, custom
interfaces, and spatio-temporal voxel costmap support for autonomous navigation.

The source tree includes the LIO-SAM package, Livox ROS 2 driver and SDK, Nav2,
rover model and navigation packages, custom interfaces, GTSAM, and the voxel
layer. Build outputs and runtime logs are intentionally excluded from Git.

## Running

```bash
ros2 launch livox_ros_driver2 msg_MID360_launch.py
ros2 launch lio_sam run.launch.py
ros2 launch rover_navigation navigation.launch.py
```
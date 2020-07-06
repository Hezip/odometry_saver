# Project Title

Store the **point cloud** and the corresponding **pose** of **each frame**

----

Forked from [koide3/odometry_saver](https://github.com/koide3/odometry_saver)

Change to fit aloam's point and odom in interactive_slam

Add service to save map(Should not be too big)

## Getting Started

```
roslaunch odometry_saver online.launch dst_directory:={folder} points_topic:={your topic}
rosbag play {your bag with points / poses}
```
save map(Point cloud accumulation, without pose)
```
rosservice call /map_saver  "/home/me/map.pcd"
```


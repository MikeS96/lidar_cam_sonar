# Mapping LiDAR point cloud to camera image frame

This repository aims to be a short guide to map LiDAR point clouds to a camera image frame in the [Kitti dataset](http://www.cvlibs.net/datasets/kitti/). 

<div  align="center">
<img  src="./assets/point_mapped.png" width="440">
</div>

## Description

Robotics-vision in a crucial task to endowing autonomous driving vehicles with environmental awareness. Without robust perception pipelines, it would be impossible to obtain reliable decision-making systems. This notebook aims to be a short guide and teach how to map a LiDAR point cloud to an image frame synchronize at the same timestamp.

<div  align="center">
<img  src="./assets/point_cloud.png" width="440">
</div>

The notebook is divided in the following sections:

 - Loading images, point clouds and transformation matrices
 - Transforming Point cloud to camera image frame
 - Filtering the point cloud and aligning

<div  align="center">
<img  src="./assets/final_point_cloud.png" width="440">
</div>

## Dependencies

 - pykitti
 - numpy
 - cv2
 - matplotlib
 - open3d
 - 
## Files
If you want to use this Notebook, please download the Kitti dataset and arrange its files as show below.

> ├── 2011_09_26
│   ├── 2011_09_26_drive_0005_sync
│   │   ├── image_00
│   │   │   ├── data [154 entries exceeds filelimit, not opening dir]
│   │   │   └── timestamps.txt
│   │   ├── image_01
│   │   │   ├── data [154 entries exceeds filelimit, not opening dir]
│   │   │   └── timestamps.txt
│   │   ├── image_02
│   │   │   ├── data [154 entries exceeds filelimit, not opening dir]
│   │   │   └── timestamps.txt
│   │   ├── image_03
│   │   │   ├── data [154 entries exceeds filelimit, not opening dir]
│   │   │   └── timestamps.txt
│   │   ├── oxts
│   │   │   ├── data [154 entries exceeds filelimit, not opening dir]
│   │   │   ├── dataformat.txt
│   │   │   └── timestamps.txt
│   │   └── velodyne_points
│   │       ├── data [154 entries exceeds filelimit, not opening dir]
│   │       ├── timestamps_end.txt
│   │       ├── timestamps_start.txt
│   │       └── timestamps.txt
│   ├── calib_cam_to_cam.txt
│   ├── calib_imu_to_velo.txt
│   └── calib_velo_to_cam.txt
├── assets
│   ├── final_point_cloud.png
│   ├── point_cloud.png
│   └── point_mapped.png
├── image_laser_fusion.ipynb
├── Raw_PointCloud_Totaltxt
└── README.md

Special thanks to [JohanSamir](https://github.com/JohanSamir) for providing this awesome notebook.


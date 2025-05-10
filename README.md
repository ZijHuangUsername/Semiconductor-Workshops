# Semiconductor Workshop RGBD Dataset

This dataset contains RGBD images for 3D reconstruction of scenes in a semiconductor workshop. The dataset is modeled using **Blender** and generated using [BlenderProc](https://github.com/DLR-RM/BlenderProc). The format of the dataset is based on the structure of the [Neural RGB-D dataset](https://github.com/dazinovic/neural-rgbd-surface-reconstruction), and it includes various data types for depth and RGB images, along with ground truth poses for camera calibration and optimization.

## Dataset Structure

The dataset follows the following directory structure:
<scene_name> # args.datadir in the config file
├── depth # Raw (real data) or ground truth (synthetic data) depth images (optional)
│ ├── depth0.png
│ ├── depth1.png
│ ├── depth2.png
│ ...
├── depth_filtered # Filtered depth images
│ ├── depth0.png
│ ├── depth1.png
│ ├── depth2.png
│ ...
├── images # RGB images
│ ├── img0.png
│ ├── img1.png
│ ├── img2.png
│ ...
├── intrinsic_depth.txt # 4x4 intrinsic camera matrix for depth images
├── poses.txt # Ground truth camera poses (optional)
├── trainval_poses.txt # Camera poses used for optimization
├── gt_mesh_culled.ply # Culled mesh of the reconstructed 3D model 

## Download Link
You can download the dataset from the following link:

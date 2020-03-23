# disparity_image_proc

Contains package that allows converting ROS disparity images to depth images.

### Usage

Checkout the launch file for the actual input/output topic names, here is an example:

```
roslaunch disparity_image_proc disparity_to_depth.launch \
  left_cam_info:=/tesse/left_cam/camera_info \
  right_cam_info:=/tesse/right_cam/camera_info \
  disparity:=/stereo_gray/disparity
```

This will output the depth image to the topic: `/disparity_image_proc/depth/image_raw`
by default.

# SemSLAM

Builds 3D map of indoor environments from RGBD images.

Pipeline

1. Segmentate every RGB image on two classes: empty (floor) and occupied
2. Read if available relative translations between this and previous images. If translations not available predict them.
3. Construct point cloud of occupied pixels in image.
4. Intergrate this local point cloud to global map.

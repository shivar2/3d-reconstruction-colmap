# 3d-reconstruction-colmap

This project demonstrates **multi-view 3D reconstruction** using [COLMAP](https://colmap.github.io/).  
The dataset used here is **DTU Scan6**, part of the [DTU Robot Image Dataset](http://roboimagedata.compute.dtu.dk/).

## 🚀 Pipeline Overview
The reconstruction process follows these main steps in COLMAP:

1. **Feature Extraction** – detect keypoints and descriptors.  
   <img src="images/feature_extraction.png" alt="Feature Extraction" width="200"/>

2. **Feature Matching** – match features across all image pairs.  
   <img src="images/feature_matching.png" alt="Feature Matching" width="300"/>

3. **Sparse Reconstruction (SfM)** – estimate camera poses and build a sparse point cloud.  
   <img src="images/sfm1.png" alt="Sparse" width="300"/>
   <img src="images/sfm2.png" alt="Sparse" width="300"/>
   <img src="images/sfm3.png" alt="Sparse" width="300"/>
   <img src="images/sfm4.png" alt="Sparse" width="300"/>

4. **Dense Reconstruction (MVS)** – create a dense point cloud from multi-view stereo.  
   <img src="images/dense1.png" alt="Dense" width="400"/>
   <img src="images/dense2.png" alt="Dense" width="400"/>
   <img src="images/dense3.png" alt="Dense" width="400"/>

5. **Final Dense point cloud**  
   <img src="images/ply1.png" alt="Mesh" width="300"/>
   <img src="images/ply2.png" alt="Mesh" width="300"/>
   <img src="images/ply3.png" alt="Mesh" width="300"/>

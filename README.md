# 3d-reconstruction-colmap

This project demonstrates **multi-view 3D reconstruction** using [COLMAP](https://colmap.github.io/).  
The dataset used here is **DTU Scan6**, part of the [DTU Robot Image Dataset](http://roboimagedata.compute.dtu.dk/).

## 🚀 Pipeline Overview
The reconstruction process follows these main steps in COLMAP:

1. **Feature Extraction** – detect keypoints and descriptors.  
   ![Feature Extraction](images/feature_extraction.png)

2. **Feature Matching** – match features across all image pairs.  
   ![Feature Matching](images/feature_matching.png)

3. **Sparse Reconstruction (SfM)** – estimate camera poses and build a sparse point cloud.  
   ![Sparse](images/sfm1.png)
   ![Sparse](images/sfm2.png)
   ![Sparse](images/sfm3.png)
   ![Sparse](images/sfm4.png)

5. **Dense Reconstruction (MVS)** – create a dense point cloud from multi-view stereo.  
   ![Dense](images/dense1.png)
   ![Dense](images/dense2.png)
   ![Dense](images/dense3.png)

7. **(Optional) Meshing** – reconstruct a surface mesh from the dense point cloud.  
   ![Mesh](images/ply1.png)
   ![Mesh](images/ply2.png)
   ![Mesh](images/ply3.png)

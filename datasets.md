# Public Datasets

## LINEMOD (LM)
- Modality: RGB-D
- Description: Proposed by Hinterstoisser et al. at ACCV 2012, LINEMOD contains 15 RGB-D sequences and more than 18,000 real images with accurate pose annotations. The scenes include cluttered backgrounds, texture-less objects, and varying illumination. As one of the earliest benchmark datasets for 6D object pose estimation, it has played an important role in the development of traditional pose estimation methods and remains a widely used benchmark in complex scenes.
- Link: [https://campar.in.tum.de/Chair/Projects/LineMod](https://ieeexplore.ieee.org/abstract/document/6042881)

## LINEMOD-Occluded (LM-O)
- Modality: RGB-D
- Description: Proposed by Brachmann et al. at ECCV 2014, LINEMOD-Occluded is an extension of the LINEMOD dataset. It introduces 8 highly occluded object samples, with occlusion rates often exceeding 70%, and constructs more challenging scenes with stacked objects and background interference. It is widely used to evaluate pose estimation robustness under severe occlusion.
- Link:[ https://bop.felk.cvut.cz/datasets/](https://link.springer.com/chapter/10.1007/978-3-319-10605-2_35)

## YCB-Video
- Modality: RGB-D
- Description: Released in 2017, YCB-Video is a large-scale RGB-D video dataset containing 92 videos and more than 130,000 frames of 21 daily objects. It provides detailed annotations including 6D poses, 2D bounding boxes, and masks. Because the scenes include clutter, illumination variation, and occlusion, it is widely used as an important benchmark for robotic vision, augmented reality, temporal consistency, and real-time pose estimation.
- Link: https://arxiv.org/abs/1711.00199

## NOCS 
- Modality: RGB-D / synthetic + real
- Description: Released by He Wang et al. at CVPR 2019, NOCS includes a synthetic training set (CAMERA) and a real test set (REAL275), with annotations of categories, 6D poses, and 2D bounding boxes. It is a representative benchmark for category-level 6D pose estimation and is widely used to evaluate generalization ability across object instances and complex scenes.
- Link: https://openaccess.thecvf.com/content_CVPR_2019/html/Wang_Normalized_Object_Coordinate_Space_for_Category-Level_6D_Object_Pose_and_CVPR_2019_paper.html
  
## Omni6DPose
- Modality: Real + synthetic
- Description: Proposed by Mengchen Zhang et al. at ECCV 2024, Omni6DPose includes a real dataset (ROPE) and a synthetic dataset (SOPE). It covers 149 categories, more than 5,000 instances, and over 800,000 images with rich annotations. Due to its scale and diversity, it is well suited for evaluating robustness and generalization in category-level pose estimation.
- Link: (https://link.springer.com/chapter/10.1007/978-3-031-73226-3_12)

## Wild6D
- Modality: Real images
- Description: Released in 2022 by the University of California, San Diego, Wild6D contains more than 1.1 million images and covers 1,722 object instances from five categories, such as bottles and bowls. It focuses on category-level 6D pose estimation in real-world scenes and provides large-scale support for pose estimation and tracking research.
- Link:https://proceedings.neurips.cc/paper_files/paper/2022/hash/afe99e55be23b3523818da1fefa33494-Abstract-Conference.html

## OnePose
- Modality: RGB / multi-scene video
- Description: Released at CVPR 2022, OnePose contains more than 450 multi-scene video sequences of 150 objects, with annotations of camera poses and 3D bounding boxes. It is specifically designed to evaluate pose estimation for unseen objects and is widely used in augmented reality and robotic manipulation scenarios.
- Link: https://openaccess.thecvf.com/content/CVPR2022/html/Sun_OnePose_One-Shot_Object_Pose_Estimation_Without_CAD_Models_CVPR_2022_paper.html

## GenMOP
- Modality: RGB / model-free benchmark
- Description: Proposed at CVPR 2022, GenMOP is designed to evaluate model-free pose estimation methods. It contains 10 objects, including planar and structured objects, and each object is associated with two video sequences captured in different environments. Camera poses are reconstructed by COLMAP, and key points are manually labeled to align sequences. It is valuable for evaluating the pose estimation ability of unseen objects in augmented reality and robotic manipulation scenarios.
- Link: https://link.springer.com/chapter/10.1007/978-3-031-19824-3_18

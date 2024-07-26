# Awesome 3D Gaussian Splatting for Robotics [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This repo contains a curative list of **3D Gaussian Splatting papers relating to the Robotics domain**.

#### Please feel free to send me [pull requests](https://github.com/dtc111111/awesome-3dgs-for-robotics) or [email](mailto:dengtianchen@sjtu.edu.cn) to add papers! <br>

If you find this repository useful, please consider [citing](#citation) and STARing this list. Feel free to share this list with others!

---

## Overview
  - [3DGS Survey](#3dgs-survey)
    
  - [3DGS Foundation Model](#3dgs-general-model)

  - [Perception](#perception)
    - [Semantic](#Semantic)
    - [Multi-Modal](#MM)
    - [Object Detection](#Object-Detection)
    
  - [Mapping & Localization](#slam)
    - [3D Reconstruction](#3D-Reconstruction)
    - [Dynamic Scene Reconstruction](#Dynamic-Reconstruction)
    - [Visual-SLAM](#Visual-SLAM)
    - [Lidar-SLAM](#Lidar-SLAM)
    - [Multimodal-SLAM](#Multimodal-SLAM)
      
  - [Planning & Navigation](#planningnavigation)
  - [Manipulation & RL](#manipulationrl)

  - [Citation](#citation)

---
## 3DGS Survey

#### [S1] A Survey on 3D Gaussian Splatting
- **🧑‍🔬 Author**：Guikun Chen, Wenguan Wang
- **🏫 Institute**：Zhejiang University
- **🔗 Link**：[[arXiv:2401.03890](https://arxiv.org/abs/2401.03890)]


#### [S2] 3D Gaussian as a New Vision Era: A Survey
- **🧑‍🔬 Author**：Ben Fei, Jingyi Xu, Rui Zhang, Qingyuan Zhou, Weidong Yang, Ying He
- **🏫 Institute**：Fudan University ⟐ Nanyang Technological University
- **🔗 Link**：[[arXiv:2402.07181](https://arxiv.org/abs/2402.07181)]


#### [S3] Recent Advances in 3D Gaussian Splatting
- **🧑‍🔬 Author**：Tong Wu, Yu-Jie Yuan, Ling-Xiao Zhang, Jie Yang, Yan-Pei Cao, Ling-Qi Yan, Lin Gao
- **🏫 Institute**：Chinese Academy of Sciences ⟐ VAST ⟐  University of California
- **🔗 Link**：[[arXiv:2403.11134](https://arxiv.org/abs/2403.11134)]


#### [S4] Gaussian Splatting: 3D Reconstruction and Novel View Synthesis, a Review
- **🧑‍🔬 Author**：Anurag Dalal, Daniel Hagen, Kjell G. Robbersmyr, Kristian Muri Knausgård
- **🏫 Institute**：University of Agder
- **🔗 Link**：[[arXiv:2405.03417](https://arxiv.org/abs/2405.03417)]

## Seminal Works in 3DGS 
* 3D Gaussian Splatting for Real-Time Radiance Field Rendering, *SIGGRAPH, 2023*. [[Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf)] [[Website](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)]
* 2D Gaussian Splatting for Geometrically Accurate Radiance Fields, *SIGGRAPH, 2024*. [[Paper](https://arxiv.org/pdf/2403.17888)] [[Website](https://surfsplatting.github.io/)]  [[Code](https://github.com/hbb1/2d-gaussian-splatting)]
* **Mip-splatting**: Alias-free 3d gaussian splatting, *CVPR, 2024*. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_Mip-Splatting_Alias-free_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)] [[Website](https://niujinshuchong.github.io/mip-splatting/)]  [[Code](https://github.com/autonomousvision/mip-splatting)]

## Mapping & Localization
### 3D Reconstruction

* SuGaR: Surface-Aligned Gaussian Splatting for Efficient 3D Mesh Reconstruction and High-Quality Mesh Rendering, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2311.12775)] [[Website](https://imagine.enpc.fr/~guedona/sugar/)]  [[Code](https://github.com/Anttwo/SuGaR)]
* 2D Gaussian Splatting for Geometrically Accurate Radiance Fields, *SIGGRAPH, 2024*. [[Paper](https://arxiv.org/pdf/2403.17888)] [[Website](https://surfsplatting.github.io/)]  [[Code](https://github.com/hbb1/2d-gaussian-splatting)]
* Gaussian Opacity Fields: Efficient and Compact Surface Reconstruction in Unbounded Scenes, *arXiv*.  [[Paper](https://arxiv.org/pdf/2404.10772)] [[Website](https://niujinshuchong.github.io/gaussian-opacity-fields/)]  [[Code](https://github.com/autonomousvision/gaussian-opacity-fields)]
* High-quality Surface Reconstruction using Gaussian Surfels, *SIGGRAPH, 2024*. [[Paper](https://arxiv.org/pdf/2404.17774
)] [[Website](https://turandai.github.io/projects/gaussian_surfels/)]  [[Code](https://github.com/turandai/gaussian_surfels)]
* RaDe-GS: Rasterizing Depth in Gaussian Splatting, *arXiv*. 
[[Paper](https://arxiv.org/pdf/2406.01467
)] [[Website](https://baowenz.github.io/radegs/)]  [[Code](https://github.com/BaowenZ/RaDe-GS)]



### Dynamic Scene Reconstruction
* EgoGaussian: Dynamic Scene Understanding from Egocentric Video with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.19811)] [[Website](https://arxiv.org/abs/2406.19811)]
* Dynamic Gaussian Marbles for Novel View Synthesis of Casual Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.18717)] [[Website](https://arxiv.org/abs/2406.18717)]
* VGD: Vision-Only Dynamic Gaussian for Driving Simulation, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.18198)] [[Website](https://arxiv.org/abs/2406.18198)]
* Modeling Ambient Scene Dynamics for Free-view Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.09395)] [[Website](https://arxiv.org/abs/2406.09395)]
* InfoGaussian: Structure-Aware Dynamic Gaussians through Lightweight Information Shaping, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.05897)] [[Website](https://arxiv.org/abs/2406.05897)]
* Dynamic 3D Gaussian Fields for Urban Areas, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.03175)] [[Website](https://tobiasfshr.github.io/pub/4dgf/)] [[Code](https://github.com/tobiasfshr/map4d)]
* Reconstructing and Simulating Dynamic 3D Objects with Mesh-adsorbed Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.01476)] [[Website](https://wcwac.github.io/MaGS-page/)] [[Code](https://github.com/wcwac/MaGS)]
* DreamPhysics: Learning Physical Properties of Dynamic 3D Gaussians with Video Diffusion Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.09395)] [[Website](https://arxiv.org/abs/2406.01476)] [[Code](https://github.com/tyhuang0428/DreamPhysics)]
* MoDGS: Dynamic Gaussian Splatting from Causually-captured Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.00434)] [[Website](https://arxiv.org/abs/2406.00434)]
* Street Gaussians for Modeling Dynamic Urban Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.01339.pdf)] [[Website](https://zju3dv.github.io/street_gaussians/)] [[Code](https://github.com/zju3dv/street_gaussians)]
* DrivingGaussian: Composite Gaussian Splatting for Surrounding Dynamic Autonomous Driving Scenes, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.07920.pdf)] [[Website](https://pkuvdig.github.io/DrivingGaussian/)]
* HUGS: Golistic Urban 3D Scene Understanding via Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.12722.pdf)] [[Website](https://xdimlab.github.io/hugs_website/)]
* Guess The Unseen: Dynamic 3D Scene Reconstruction from Partial 2D Glimpses, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2404.14410)] [[Website](https://snuvclab.github.io/gtu/)] [[Code](https://github.com/snuvclab/gtu/)]

## Planning & Navigation
* GaussNav: Gaussian Splatting for Visual Navigation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11625.pdf)] [[Website](https://xiaohanlei.github.io/projects/GaussNav/)] [[Code](https://github.com/XiaohanLei/GaussNav)]
* 3DGS-ReLoc: 3D Gaussian Splatting for Map Representation and Visual ReLocalization, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11367)] [[Website](https://arxiv.org/abs/2403.11367)]
* Beyond Uncertainty: Risk-Aware Active View Acquisition for Safe Robot Navigation and 3D Scene Understanding with FisherRF, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11396)] [[Website](https://arxiv.org/abs/2403.11396)]
* 3DGS-Calib: 3D Gaussian Splatting for Multimodal SpatioTemporal Calibration, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11577)] [[Website](https://arxiv.org/abs/2403.11577)]
* HO-Gaussian: Hybrid Optimization of 3D Gaussian Splatting for Urban Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20032.pdf)] [[Website](https://arxiv.org/abs/2403.20032)]
* SGD: Street View Synthesis with Gaussian Splatting and Diffusion Prior, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20079.pdf)] [[Website](https://arxiv.org/abs/2403.20079)]
---
## Citation

If you find this repository useful, please consider citing this list:

```
@misc{Deng20243dgspaperlist,
    title = {awesome-Implicit-NeRF-SLAM},
    author = {Tianchen Deng, Yue Pan, Xingxing Zuo, Shenghai Yuan, Nailin Wang, Hesheng Wang, Jingchuan Wang, Lihua Xie, Danwei Wang, Weidong Chen},
    howpublished = {\url{https://github.com/dtc111111/awesome-3dgs-for-robotics}},
    year = {2024}
}
```

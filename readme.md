<div align="center"> 
<img src="Images/image1.png" width="400" height="350" alt="Celebration"/>    
   
# Awesome 3D Gaussian Splatting for Robotics [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
   
 


This repo contains a curative list of **3D Gaussian Splatting papers relating to the Robotics domain**.

#### Please feel free to send me [pull requests](https://github.com/dtc111111/awesome-3dgs-for-robotics) or [email](mailto:dengtianchen@sjtu.edu.cn) to add papers! <br>

If you find this repository useful, please consider [citing](#citation) and STARing this list. Feel free to share this list with others!
<div align="left">   
  
---

## Overview
  - [3DGS Survey](#3dgs-survey)
    
  - [3DGS General Model](#3dgs-general-model)
    - [Photorealistic](#photorealistic)
    - [Sparse View](#sparse-view)
    - [Accelerate & Compression](#accelerate--compression)
    - [Geometry & Physics](#Geometry--Physics)

  - [Perception](#perception)
    - [Semantic](#semantic)
    - [Multi-Modal](#Multi-Modal)
    - [Relightable & Complex Environment & Rainy](#relightable--complex-environment--rainy)
    
  - [Mapping & Localization](#mapping--localization)
    - [3D Reconstruction](#3d-reconstruction)
    - [Dynamic Scene Reconstruction](#dynamic-scene-reconstruction)
    - [Localization & Visual SLAM](#localization--visual-slam)
    - [Multimodal-SLAM](#multimodal-slam)
      
  - [Planning & Navigation](#planning--navigation)
  - [Manipulation & RL](#manipulation--rl)
  - [Simulation & Human Interaction](#simulation--generation)

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
- **🔗 Link**：[[IEEE Transactions on Visualization and Computer Graphics 2024](https://arxiv.org/abs/2402.07181)]


#### [S3] Recent Advances in 3D Gaussian Splatting
- **🧑‍🔬 Author**：Tong Wu, Yu-Jie Yuan, Ling-Xiao Zhang, Jie Yang, Yan-Pei Cao, Ling-Qi Yan, Lin Gao
- **🏫 Institute**：Chinese Academy of Sciences ⟐ VAST ⟐  University of California
- **🔗 Link**：[[arXiv:2403.11134](https://arxiv.org/abs/2403.11134)]


#### [S4] Gaussian Splatting: 3D Reconstruction and Novel View Synthesis, a Review
- **🧑‍🔬 Author**：Anurag Dalal, Daniel Hagen, Kjell G. Robbersmyr, Kristian Muri Knausgård
- **🏫 Institute**：University of Agder
- **🔗 Link**：[[IEEE Access](https://arxiv.org/abs/2405.03417)]


#### [S5] Survey on Fundamental Deep Learning 3D Reconstruction Techniques
- **🧑‍🔬 Author**：Yonge Bai, LikHang Wong, TszYin Twan
- **🏫 Institute**：McMaster University ⟐  City University of Hong Kong
- **🔗 Link**：[[arXiv:2405.03417](https://arxiv.org/abs/2407.08137)]


#### [S6] 3D Gaussian Splatting: Survey, Technologies, Challenges, and Opportunities
- **🧑‍🔬 Author**：Yanqi Bao, Tianyu Ding, Jing Huo, Yaoli Liu, Yuxin Li, Wenbin Li, Yang Gao, Jiebo Luo
- **🏫 Institute**：Nanjing University ⟐  University of Rochester ⟐ Microsoft
- **🔗 Link**：[[arXiv:2405.03417](https://arxiv.org/abs/2407.17418)]




## 3DGS General Model
---
* 3D Gaussian Splatting for Real-Time Radiance Field Rendering, **SIGGRAPH, 2023**. [[Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf)] [[Website](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)]
### Photorealistic
* Mip-splatting Alias-free 3d gaussian splatting, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_Mip-Splatting_Alias-free_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)] [[Website](https://niujinshuchong.github.io/mip-splatting/)]  [[Code](https://github.com/autonomousvision/mip-splatting)]
* End-to-End Rate-Distortion Optimized 3D Gaussian Representation, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2406.01597.pdf)] [[Website](https://arxiv.org/abs/2406.01597)] [[Code](https://github.com/USTC-IMCL/RDO-Gaussian)]
* Analytic-Splatting: Anti-Aliased 3D Gaussian Splatting via Analytic Integration, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11056.pdf)]
* Learn to Optimize Denoising Scores for 3D Generation: A Unified and Improved Diffusion Prior on NeRF and 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.04820)] [[Code](https://github.com/yangxiaofeng/LODS)]
* Deblurring 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2401.00834)] [[Code](https://github.com/benhenryL/Deblurring-3D-Gaussian-Splatting)]
* BAD-Gaussians: Bundle Adjusted Deblur Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.11831)] [[Code](https://github.com/WU-CVGL/BAD-Gaussians)]
* MIGS: Multi-Identity Gaussian Splatting via Tensor Decomposition, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2407.07284)]
* Multi-Scale 3D Gaussian Splatting for Anti-Aliased Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.17089.pdf)]
* Implicit Gaussian Splatting with Efficient Multi-Level Tri-Plane Representation, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.10041)]
* GaussianPro: 3D Gaussian Splatting with Progressive Propagation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.14650.pdf)] [[Website](https://kcheng1021.github.io/gaussianpro.github.io/)] [[Code](https://github.com/kcheng1021/GaussianPro)]
* RayGauss: Volumetric Gaussian-Based Ray Casting for Photorealistic Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/abs/2408.03356)]
* Spec-Gaussian: Anisotropic View-Dependent Appearance for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.15870.pdf)]
* Gaussian Splatting with Localized Points Management, *arXiv*. [[Paper](https://arxiv.org/abs/2406.04251)]
---

### Sparse View
* Fast Dynamic 3D Object Generation from a Single-view Video, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.08742.pdf)] [[Website](https://fudan-zvg.github.io/Efficient4D/)] [[Code](https://github.com/fudan-zvg/Efficient4D)]
* GaussianObject: Just Taking Four Images to Get A High-Quality 3D Object with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.10259.pdf)] [[Website](https://gaussianobject.github.io/)] [[Code](https://github.com/GaussianObject/GaussianObject)]
* LGM: Large Multi-View Gaussian Model for High-Resolution 3D Content Creation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.05054.pdf)] [[Website](https://me.kiui.moe/lgm/)] [[Code](https://github.com/3DTopia/LGM)]
* IM-3D: Iterative Multiview Diffusion and Reconstruction for High-Quality 3D Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.08682.pdf)] [[Website](https://arxiv.org/abs/2402.08682)]
* FDGaussian: Fast Gaussian Splatting from Single Image via Geometric-aware Diffusion Model, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10242.pdf)] [[Website](https://qjfeng.net/FDGaussian)]
* Depth-Regularized Optimization for 3D Gaussian Splatting in Few-Shot Images, **CVPRW, 2024**. [[Paper](https://arxiv.org/pdf/2311.13398.pdf)] [[Website](https://robot0321.github.io/DepthRegGS/index.html)] [[Coda](https://github.com/robot0321/DepthRegularizedGS)]
* DNGaussian: Optimizing Sparse-View 3D Gaussian Radiance Fields with Global-Local Depth Normalization, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.06912.pdf)] [[Website](https://fictionarry.github.io/DNGaussian/)] [[Coda](https://github.com/Fictionarry/DNGaussian)]
* MVSplat: Efficient 3D Gaussian Splatting from Sparse Multi-View Images, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.14627)] [[Website](https://donydchen.github.io/mvsplat/)] [[Coda](https://github.com/donydchen/mvsplat)]
* latentSplat: Autoencoding Variational Gaussians for Fast Generalizable 3D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.16292.pdf)] [[Website](https://geometric-rl.mpi-inf.mpg.de/latentsplat/)] [[Coda](https://github.com/Chrixtar/latentsplat)]
* GRM: Large Gaussian Reconstruction Model for Efficient 3D Reconstruction and Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14621.pdf)] [[Website](https://justimyhxu.github.io/projects/grm/)] [[Coda](https://github.com/justimyhxu/grm)]
* Gamba: Marry Gaussian Splatting with Mamba for single view 3D reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.18795)]
* CoherentGS: Sparse Novel View Synthesis with Coherent 3D Gaussians, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.19495)] [[Website](https://people.engr.tamu.edu/nimak/Papers/CoherentGS/index.html)]
* InstantSplat: Unbounded Sparse-view Pose-free Gaussian Splatting in 40 Seconds, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20309.pdf)] [[Website](https://instantsplat.github.io/)]
* Sp<sup>2</sup>360: Sparse-view 360 Scene Reconstruction using Cascaded 2D Diffusion Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.16517)]
* SparseGS: Real-Time 360° Sparse View Synthesis using Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00206.pdf)] [[Website](https://formycat.github.io/SparseGS-Real-Time-360-Sparse-View-Synthesis-using-Gaussian-Splatting/)]
* FSGS: Real-Time Few-shot View Synthesis using Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.00451.pdf)] [[Website](https://zehaozhu.github.io/FSGS/)] [[Coda](https://github.com/VITA-Group/FSGS)]
* pixelSplat: 3D Gaussian Splats from Image Pairs for Scalable Generalizable 3D Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.12337.pdf)] [[Website](https://davidcharatan.com/pixelsplat/)] [[Coda](https://github.com/dcharatan/pixelsplat)]
* Splatter Image: Ultra-Fast Single-View 3D Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.13150.pdf)] [[Website](https://szymanowiczs.github.io/splatter-image.html)] [[Coda](https://github.com/szymanowiczs/splatter-image)]
* EndoSparse: Real-Time Sparse View Synthesis of Endoscopic Scenes using Gaussian Splatting, **MICCAI, 2024**. [[Paper](https://arxiv.org/abs/2407.01029)] [[Code](https://github.com/CUHK-AIM-Group/EndoSparse)]
* Learning 3D Gaussians for Extremely Sparse-View Cone-Beam CT Reconstruction, **MICCAI, 2024**. [[Paper](https://arxiv.org/abs/2407.01090)] [[Code](https://github.com/xmed-lab/DIF-Gaussian)]
* CoR-GS: Sparse-View 3D Gaussian Splatting via Co-Regularization, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2405.12110)]
* LoopSparseGS: Loop Based Sparse-View Friendly Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.00254)]
* Self-augmented Gaussian Splatting with Structure-aware Masks for Sparse-view 3D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.04831)]
* ReconX: Reconstruct Any Scene from Sparse Views with Video Diffusion Model, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.16767)]
* LM-Gaussian: Boost Sparse-view 3D Gaussian Splatting with Large Model Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.03456)]
* Optimizing 3D Gaussian Splatting for Sparse Viewpoint Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.03213)]
* Object Gaussian for Monocular 6D Pose Estimation from Sparse Views, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.02581)]
* Single-View 3D Reconstruction via SO(2)-Equivariant Gaussian Sculpting Networks, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.07245)]
* Vista3D: Unravel the 3D Darkside of a Single Image, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12193)]
* MVPGS: Excavating Multi-view Priors for Gaussian Splatting from Sparse Input Views, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.14316)]
* Self-Evolving Depth-Supervised 3D Gaussian Splatting from Rendered Stereo Pairs, **BMVC 2024**. [[Paper](https://arxiv.org/abs/2409.07456)]
* Frequency-based View Selection in Gaussian Splatting Reconstruction, *arXiv*. [[Paper](https://arxiv.org/abs/2409.16470)]
* GSD: View-Guided Gaussian Splatting Diffusion for 3D Reconstruction, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.04237)]

### Accelerate & Compression
* Hash3D: Training-free Acceleration for 3D Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.06091)] [[Website](https://adamdad.github.io/hash3D/)] [[Code](https://github.com/Adamdad/hash3D)]
* Characterizing Satellite Geometry via Accelerated 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.02588.pdf)]
* TRIPS: Trilinear Point Splatting for Real-Time Radiance Field Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.06003.pdf)] [[Website](https://lfranke.github.io/trips/)] [[Code](https://github.com/lfranke/trips)]
* GaussianImage: 1000 FPS Image Representation and Compression by 2D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08551)]
* TOGS: Gaussian Splatting with Temporal Opacity Offset for Real-Time 4D DSA Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.19586)]
* Periodic Vibration Gaussian: Dynamic Urban Scene Reconstruction and Real-time Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.18561.pdf)] [[Website](https://fudan-zvg.github.io/PVG/)] [[Code](https://github.com/fudan-zvg/PVG)]
* Triplane Meets Gaussian Splatting: Fast and Generalizable Single-View 3D Reconstruction with Transformers, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.09147.pdf)] [[Website](https://zouzx.github.io/TriplaneGaussian/)] [[Code](https://github.com/VAST-AI-Research/TriplaneGaussian)]
* DISTWAR: Fast Differentiable Rendering on Raster-based Rendering Pipelines, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.05345.pdf)]
* FreGS: 3D Gaussian Splatting with Progressive Frequency Regularization, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.06908.pdf)]
* EAGLES: Efficient Accelerated 3D Gaussians with Lightweight EncodingS, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.04564.pdf)] [[Website](https://efficientgaussian.github.io/)] [[Code](https://github.com/Sharath-girish/efficientgaussian)]
* Optimal Projection for 3D Gaussian Splatting, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2402.00752.pdf)]
* StopThePop: Sorted Gaussian Splatting for View-Consistent Real-time Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.00525.pdf)] [[Website](https://r4dl.github.io/StopThePop/)] [[Code](https://github.com/r4dl/StopThePop)]
* GES: Generalized Exponential Splatting for Efficient Radiance Field Rendering, *CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2402.10128.pdf)] [[Website](https://abdullahamdi.com/ges/)] [[Code](https://github.com/ajhamdi/ges-splatting)]
* Identifying Unnecessary 3D Gaussians using Clustering for Fast Rendering of 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.13827.pdf)]
* RadSplat: Radiance Field-Informed Gaussian Splatting for Robust Real-Time Rendering with 900+ FPS, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.13806.pdf)] [[Website](https://m-niemeyer.github.io/radsplat/)]
* Mini-Splatting: Representing Scenes with a Constrained Number of Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14166.pdf)]
* Pixel-GS: Density Control with Pixel-aware Gradient for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.15530.pdf)]
* Octree-GS: Towards Consistent Real-time Rendering with LOD-Structured 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.17898)] [[Website](https://city-super.github.io/octree-gs/)] [[Code](https://github.com/city-super/Octree-GS)]
* SA-GS: Scale-Adaptive Gaussian Splatting for Training-Free Anti-Aliasing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.19615)] [[Website](https://kevinsong729.github.io/project-pages/SA-GS/)] [[Code](https://github.com/zsy1987/SA-GS/)]
* OmniGS: Omnidirectional Gaussian Splatting for Fast Radiance Field Reconstruction using Omnidirectional Images, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.03202)]
* GSCore: Efficient Radiance Field Rendering via Architectural Support for 3D Gaussian Splatting, *arXiv*. [[Paper](https://jaewoong.org/pubs/asplos24-gscore.pdf)]
* Scaffold-GS: Structured 3D Gaussians for View-Adaptive Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.00109.pdf)] [[Website](https://city-super.github.io/scaffold-gs/)] [[Code](https://github.com/city-super/Scaffold-GS)]
* Superpoint Gaussian Splatting for Real-Time High-Fidelity Dynamic Scene Reconstruction, **ICML, 2024**. [[Paper](https://arxiv.org/pdf/2406.03697)]
* FastScene: Text-Driven Fast 3D Indoor Scene Generation via Panoramic Gaussian Splatting, **IJCAI, 2024**. [[Paper](https://arxiv.org/abs/2405.05768)]
* Compressed 3D Gaussian Splatting for Accelerated Novel View Synthesis, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2401.02436)] [[Code](https://github.com/KeKsBoTer/c3dgs)]
* Compact3D: Smaller and Faster Gaussian Splatting with Vector Quantization, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2311.18159)] [[Code](https://github.com/UCDvision/compact3d)]
* HAC: Hash-grid Assisted Context for 3D Gaussian Splatting Compression, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2403.14530)] [[Code](https://github.com/YihangChen-ee/HAC)]
* GaussReg: Fast 3D Registration with Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2407.05254)]
* Compact 3D Gaussian Representation for Radiance Field, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2311.13681)] [[Code](https://github.com/maincold2/Compact-3DGS)]
* Fast Generalizable Gaussian Splatting Reconstruction from Multi-View Stereo, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2405.12218)] [[Code](https://github.com/TQTQliu/MVSGaussian)]
* MVG-Splatting: Multi-View Guided Gaussian Splatting with Adaptive Quantile-Based Geometric Consistency Densification, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2407.11840.pdf)]
* Splatfacto-W: A Nerfstudio Implementation of Gaussian Splatting for Unconstrained Photo Collections, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2407.12306.pdf)]
* 3iGS: Factorised Tensorial Illumination for 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2408.03753)]
* Compact 3D Gaussian Splatting for Static and Dynamic Radiance Fields, *arXiv*. [[Paper](https://arxiv.org/abs/2408.03822)]
* FLoD: Integrating Flexible Level of Detail into 3D Gaussian Splatting for Customizable Rendering, *arXiv*. [[Paper](https://arxiv.org/abs/2408.12894)]
* Robust 3D Gaussian Splatting for Novel View Synthesis in Presence of Distractors, *arXiv*. [[Paper](https://arxiv.org/abs/2408.11697)]
* PRoGS: Progressive Rendering of Gaussian Splats, *arXiv*. [[Paper](https://arxiv.org/abs/2409.01761)]
* Weight Conditioning for Smooth Optimization of Neural Networks, *arXiv*. [[Paper](https://arxiv.org/abs/2409.03424)]
* 3DGS-LM: Faster Gaussian-Splatting Optimization with Levenberg-Marquardt, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12892)]
* Spectral-GS: Taming 3D Gaussian Splatting with Spectral Entropy, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12771)]
* GStex: Per-Primitive Texturing of 2D Gaussian Splatting for Decoupled Appearance and Geometry Modeling, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12954)]
* MesonGS: Post-training Compression of 3D Gaussians via Efficient Attribute Transformation, *arXiv*. [[Paper](https://arxiv.org/abs/2409.09756)]

### Geometry & Physics
* 2D Gaussian Splatting for Geometrically Accurate Radiance Fields, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2403.17888)] [[Website](https://surfsplatting.github.io/)]  [[Code](https://github.com/hbb1/2d-gaussian-splatting)]
* Gaussian Splashing: Dynamic Fluid Synthesis with Gaussian Splatting, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2401.15318.pdf)] [[Website](https://amysteriouscat.github.io/GaussianSplashing/)]
* GaMeS: Mesh-Based Adapting and Modification of Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.01459.pdf)] [[Code](https://github.com/waczjoan/gaussian-mesh-splatting)]
* Mesh-based Gaussian Splatting for Real-time Large-scale Deformation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.04796.pdf)]
* Reconstruction and Simulation of Elastic Objects with Spring-Mass 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09434)] [[Website](https://zlicheng.com/spring_gaus/)] [[Code](https://github.com/Colmar-zlicheng/Spring-Gaus)]
* Texture-GS: Disentangling the Geometry and Texture for 3D Gaussian Splatting Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10050)] [[Website](https://slothfulxtx.github.io/TexGS/)] [[Code](https://github.com/slothfulxtx/Texture-GS)]
* DN-Splatter: Depth and Normal Priors for Gaussian Splatting and Meshing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.17822)] [[Website](https://maturk.github.io/dn-splatter/)] [[Code](https://github.com/maturk/dn-splatter)]
* Feature Splatting: Language-Driven Physics-Based Scene Synthesis and Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.01223)] [[Website](https://feature-splatting.github.io/)] [[Code](https://github.com/vuer-ai/feature_splatting)]
* Surface Reconstruction from Gaussian Splatting via Novel Stereo Views, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2404.01810)] [[Website](https://gs2mesh.github.io/)]
* RaDe-GS: Rasterizing Depth in Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.01467)] [[Website](https://baowenz.github.io/radegs/)]
* Trim 3D Gaussian Splatting for Accurate Geometry Representation, *arXiv*. [[Paper](https://arxiv.org/abs/2406.07499)] [[Website](https://trimgs.github.io/)] [[Code](https://github.com/YuxueYang1204/TrimGS)]
* Effective Rank Analysis and Regularization for Enhanced 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2406.11672)] [[Website](https://junhahyung.github.io/erankgs.github.io/)]
* PhysGaussian: Physics-Integrated 3D Gaussians for Generative Dynamics, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.12198.pdf)] [[Website](https://xpandora.github.io/PhysGaussian/)] [[Code](https://github.com/XPandora/PhysGaussian)]
* SuGaR: Surface-Aligned Gaussian Splatting for Efficient 3D Mesh Reconstruction and High-Quality Mesh Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.12775.pdf)] [[Website](https://imagine.enpc.fr/~guedona/sugar/)] [[Code](https://github.com/Anttwo/SuGaR)]
* NeuSG: Neural Implicit Surface Reconstruction with 3D Gaussian Splatting Guidance, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00846.pdf)]
* Projecting Radiance Fields to Mesh Surfaces, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/abs/2406.11570)]
* GeoGaussian: Geometry-aware Gaussian Splatting for Scene Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11324.pdf)]
* Enhancement of 3D Gaussian Splatting using Raw Mesh for Photorealistic Recreation of Architectures, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.15435.pdf)]
* Integrating Meshes and 3D Gaussians for Indoor Scene Reconstruction with SAM Mask Guidance, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.16173.pdf)]
* 2DGH: 2D Gaussian-Hermite Splatting for High-quality Rendering and Better Geometry Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.16982.pdf)]
* Depth Estimation Based on 3D Gaussian Splatting Siamese Defocus, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12323.pdf)]




## Perception
### Semantic
* Semantic Gaussians: Open-Vocabulary Scene Understanding with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.15624)] [[Website
](https://semantic-gaussians.github.io/)]
* Segment Any 3D Gaussians, *arXiv*. [[Paper](https://jumpat.github.io/SAGA/SAGA_paper.pdf)] [[Website](https://jumpat.github.io/SAGA/)] [[Code](https://github.com/Jumpat/SegAnyGAussians)]
* 2D-Guided 3D Gaussian Segmentation, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.16047.pdf)]
* GaussianFormer: Scene as Gaussians for Vision-Based 3D Semantic Occupancy Prediction, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2405.17429)] [[Code](https://github.com/huang-yh/GaussianFormer)]
* Click-Gaussian: Interactive Segmentation to Any 3D Gaussians, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.11793)]
* Query-based Semantic Gaussian Field for Scene Representation in Reinforcement Learning, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.02370)]
* GOI: Find 3D Gaussians of Interest with an Optimizable Open-vocabulary Semantic-space Hyperplane, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.17596)]
* Gaussian Control with Hierarchical Semantic Graphs in 3D Human Recovery, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.12477)]
* SlingBAG: Sliding ball adaptive growth algorithm with differentiable radiation enables super-efficient iterative 3D photoacoustic image reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.11781)]
* GaussianBeV: 3D Gaussian Representation meets Perception Models for BeV Segmentation, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.14108)]
* SpectralGaussians: Semantic, spectral 3D Gaussian splatting for multi-spectral scene representation, visualization and analysis, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.06975)]
* Contrastive Gaussian Clustering: Weakly Supervised 3D Scene Segmentation, *arXiv*. [[Paper](https://arxiv.org/abs/2404.12784)]
* CoSSegGaussians: Compact and Swift Scene Segmenting 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.05925.pdf)] [[Website](https://david-dou.github.io/CoSSegGaussians/)] [[Code](https://DavidDou.github.io/CoSSegGaussians)]
* Segment Anything in 3D Gaussians, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2401.17857.pdf)]
* Gaussian Grouping: Segment and Edit Anything in 3D Scenes, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.00732.pdf)] [[Code](https://github.com/lkeab/gaussian-grouping)]
* GS-PT: Exploiting 3D Gaussian Splatting for Comprehensive Point Cloud Understanding via Self-supervised Learning, *arXiv*. [[Paper](https://arxiv.org/abs/2409.04963)]
* FlashSplat: 2D to 3D Gaussian Splatting Segmentation Solved Optimally, *arXiv*. [[Paper](https://arxiv.org/abs/2409.08270)]
* Semantics-Controlled Gaussian Splatting for Outdoor Scene Reconstruction and Rendering in Virtual Reality, *arXiv*. [[Paper](https://arxiv.org/abs/2409.15959)]
* SRIF: Semantic Shape Registration Empowered by Diffusion-based Image Morphing and Flow Estimation, *arXiv*. [[Paper](https://arxiv.org/abs/2409.11682)]
* Gradient-Driven 3D Segmentation and Affordance Transfer in Gaussian Splatting Using 2D Masks, *arXiv*. [[Paper](https://arxiv.org/abs/2409.11681)]


### Multi-Modal
* Language Embedded 3D Gaussians for Open-Vocabulary Scene Understanding, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.18482.pdf)] [[Website](https://buaavrcg.github.io/LEGaussians/)] [[Code](https://github.com/buaavrcg/LEGaussians)]
* Feature 3DGS: Supercharging 3D Gaussian Splatting to Enable Distilled Feature Fields, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.03203.pdf)] [[Website](https://feature-3dgs.github.io/)] [[Code](https://github.com/ShijieZhou-UCLA/feature-3dgs)]
* LangSplat: 3D Language Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.16084.pdf)] [[Website](https://langsplat.github.io/)] [[Code](https://github.com/minghanqin/LangSplat)]
* FMGS: Foundation Model Embedded 3D Gaussian Splatting for Holistic 3D Scene Understanding,**IJCV**. [[Paper](https://arxiv.org/pdf/2401.01970.pdf)]
* Touch-GS: Visual-Tactile Supervised 3D Gaussian Splatting, **IROS 2024**. [[Paper](https://arxiv.org/pdf/2403.09875.pdf)] [[Website](https://armlabstanford.github.io/touch-gs)]
* EgoLifter: Open-world 3D Segmentation for Egocentric Perception, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.18118.pdf)] [[Website](https://egolifter.github.io/)]
* Gaga: Group Any Gaussians via 3D-aware Memory Bank, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.07977.pdf)] [[Website](https://www.gaga.gallery/)] [[Code](https://github.com/weijielyu/Gaga)]
* EvGGS: A Collaborative Learning Framework for Event-based Generalizable Gaussian Splatting, **ICML, 2024**. [[Paper](https://arxiv.org/pdf/2405.14959.pdf)]
* FastLGS: Speeding up Language Embedded Gaussians with Feature Grid Mapping, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.01916.pdf)]
* A General Framework to Boost 3D GS Initialization for Text-to-3D Generation by Lexical Richness, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.01269.pdf)]
* Event3DGS: Event-Based 3D Gaussian Splatting for High-Speed Robot Egomotion, *arXiv*. [[Paper](https://arxiv.org/abs/2406.02972)]
* Language-Embedded Gaussian Splats (LEGS): Incrementally Building Room-Scale Representations with a Mobile Robot, *arXiv*. [[Paper](https://arxiv.org/abs/2409.18108)]
* EaDeblur-GS: Event assisted 3D Deblur Reconstruction with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.13520.pdf)]

### Relightable & Complex Environment & Rainy
* DarkGS: Learning Neural Illumination and 3D Gaussians Relighting for Robotic Exploration in the Dark, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10814)] [[Code](https://github.com/tyz1030/darkgs)]
* RAIN-GS: Relaxing Accurate Initialization Constraint for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09413)] [[Website](https://ku-cvlab.github.io/RAIN-GS/)] [[Code](https://github.com/KU-CVLAB/RAIN-GS)]
* Gaussian Shadow Casting for Neural Characters, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2401.06116.pdf)]
* SWAG: Splatting in the Wild images with Appearance-conditioned Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10427.pdf)]
* Gaussian in the Wild: 3D Gaussian Splatting for Unconstrained Image Collections, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.15704)] [[Website](https://eastbeanzhang.github.io/GS-W/)] [[Code](https://github.com/EastbeanZhang/Gaussian-Wild)]
* Relightable 3D Gaussian: Real-time Point Cloud Relighting with BRDF Decomposition and Ray Tracing, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.16043.pdf)] [[Website](https://nju-3dv.github.io/projects/Relightable3DGaussian/)] [[Code](https://github.com/NJU-3DV/Relightable3DGaussian)]
* GS-IR: 3D Gaussian Splatting for Inverse Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.16473.pdf)] [[Website](https://github.com/lzhnb/GS-IR)] [[Code](https://github.com/lzhnb/GS-IR)]
* GIR: 3D Gaussian Inverse Rendering for Relightable Scene Factorization, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.05133)] [[Website](https://3dgir.github.io/)]
* LumiGauss: High-Fidelity Outdoor Relighting with 2D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.04474)]
* PRTGS: Precomputed Radiance Transfer of Gaussian Splats for Real-Time High-Quality Relighting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.03538)]
* DeRainGS: Gaussian Splatting for Enhanced Scene Reconstruction in Rainy Environments, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.11540)]
* Gaussian in the Dark: Real-Time View Synthesis From Inconsistent Dark Images Using Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.09130)]
* Phys3DGS: Physically-based 3D Gaussian Splatting for Inverse Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10335)]
* SeaSplat: Representing Underwater Scenes with 3D Gaussian Splatting and a Physically Grounded Image Formation Model, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.17345)]


## Mapping & Localization
### 3D Reconstruction
* VastGaussian: Vast 3D Gaussians for Large Scene Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2402.17427.pdf)] [[Website](https://vastgaussian.github.io/)] [[Code](https://github.com/kangpeilun/VastGaussian)]
* 3DGSR: Implicit Surface Reconstruction with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.00409.pdf)] [[Code](https://github.com/CVMI-Lab/3DGSR)]
* HGS-Mapping: Online Dense Mapping Using Hybrid Gaussian Representation in Urban Scenes, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.20159.pdf)]
* A Hierarchical 3D Gaussian Representation for Real-Time Rendering of Very Large Datasets, **SIGGRAPH, 2024**. [[Paper](https://repo-sam.inria.fr/fungraph/hierarchical-3d-gaussians/hierarchical-3d-gaussians_high.pdf)] [[Website](https://repo-sam.inria.fr/fungraph/hierarchical-3d-gaussians/)]
* Fed3DGS: Scalable 3D Gaussian Splatting with Federated Learning, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11460)] [[Code](https://github.com/DensoITLab/Fed3DGS)]
* Creating Seamless 3D Maps Using Radiance Fields, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11364.pdf)]
* CityGaussian: Real-time High-quality Large-Scale Scene Rendering with Gaussians, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.20159.pdf)] [[Website](https://dekuliutesla.github.io/citygs/)]
* MM-Gaussian: 3D Gaussian-based Multi-modal Fusion for Localization and Reconstruction in Unbounded Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.04026)]
* On Scaling Up 3D Gaussian Splatting Training, *arXiv*. [[Paper](https://arxiv.org/abs/2406.18533)] [[Website](https://daohanlu.github.io/scaling-up-3dgs/)] [[Code](https://github.com/nyu-systems/Grendel-GS)]
* HUGS: Holistic Urban 3D Scene Understanding via Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.12722.pdf)] [[Code](https://xdimlab.github.io/hugs_website/)]
* SGD: Street View Synthesis with Gaussian Splatting and Diffusion Prior, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20079.pdf)] [[Website](https://arxiv.org/abs/2403.20079)]
* Ev-GS: Event-based Gaussian splatting for Efficient and Accurate Radiance Field Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.11343.pdf)]
* GSLoc: Efficient Camera Pose Refinement via 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.11085.pdf)]
* GSFusion: Online RGB-D Mapping Where Gaussian Splatting Meets TSDF Fusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.12677.pdf)]
* LoopSplat: Loop Closure by Registering 3D Gaussian Splats, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.10154.pdf)]
* FlashGS: Efficient 3D Gaussian Splatting for Large-scale and High-resolution Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.07967.pdf)]
* OmniRe: Omni Urban Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.16760.pdf)]
* GigaGS: Scaling up Planar-Based 3D Gaussians for Large Scene Surface Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.06685.pdf)]
* LI-GS: Gaussian Splatting with LiDAR Incorporated for Accurate Large-Scale Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12899.pdf)]
* GaRField++: Reinforced Gaussian Radiance Fields for Large-Scale 3D Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12774.pdf)]
* EdgeGaussians -- 3D Edge Mapping via Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2409.12886)]
* DrivingForward: Feed-forward 3D Gaussian Splatting for Driving Scene Reconstruction from Flexible Surround-view Input, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12753)]
* RenderWorld: World Model with Self-Supervised 3D Label, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.11356)]
* Drone-assisted Road Gaussian Splatting with Cross-view Uncertainty, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.15242)]
* GGS: Generalizable Gaussian Splatting for Lane Switching in Autonomous Driving, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.02382)]

### Dynamic Scene Reconstruction
* 4Real: Towards Photorealistic 4D Scene Generation via Video Diffusion Models, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.07472.pdf)] [[Website](https://snap-research.github.io/4Real/)]
* SC4D: Sparse-Controlled Video-to-4D Generation and Motion Transfer, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.03736)] [[Website](https://sc4d.github.io/)] [[Code](https://github.com/JarrentWu1031/SC4D)]
* STAG4D: Spatial-Temporal Anchored Generative 4D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14939)] [[Website](https://nju-3dv.github.io/projects/STAG4D/)] [[Code](https://github.com/zeng-yifei/STAG4D)]
* TCLC-GS: Tightly Coupled LiDAR-Camera Gaussian Splatting for Surrounding Autonomous Driving Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.02410.pdf)] [[Website](https://arxiv.org/abs/2404.02410)]
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
* 4D Gaussian Splatting: Towards Efficient Novel View Synthesis for Dynamic Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.03307)] [[Website](https://arxiv.org/abs/2402.03307)]
* GaussianFlow: Splatting Gaussian Dynamics for 4D Content Creation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.12365)] [[Website](https://zerg-overmind.github.io/GaussianFlow.github.io/)] [[Code](https://github.com/Zerg-Overmind/GaussianFlow)]
* Motion-aware 3D Gaussian Splatting for Efficient Dynamic Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11447)] [[Website](https://arxiv.org/abs/2403.11447)]
* Bridging 3D Gaussian and Mesh for Freeview Video Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11453)] [[Website](https://arxiv.org/abs/2403.11453)]
* Per-Gaussian Embedding-Based Deformation for Deformable 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2404.03613)] [[Website](https://jeongminb.github.io/e-d3dgs/)] [[Code](https://github.com/JeongminB/E-D3DGS)]
* 3D Geometry-aware Deformable Gaussian Splatting for Dynamic View Synthesis, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2404.06270)] [[Website](https://npucvr.github.io/GaGS/)]
* Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis, **3DV, 2024**. [[Paper](https://dynamic3dgaussians.github.io/paper.pdf)] [[Website](https://dynamic3dgaussians.github.io/)] [[Code](https://github.com/JonathonLuiten/Dynamic3DGaussians)]
* Deformable 3D Gaussians for High-Fidelity Monocular Dynamic Scene Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2309.13101.pdf)] [[Website](https://ingra14m.github.io/Deformable-Gaussians/)] [[Code](https://github.com/ingra14m/Deformable-3D-Gaussians)]
* 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2310.08528.pdf)] [[Website](https://guanjunwu.github.io/4dgs/)] [[Code](https://github.com/hustvl/4DGaussians)]
* Real-time Photorealistic Dynamic Scene Representation and Rendering with 4D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2310.10642.pdf)] [[Website](https://github.com/fudan-zvg/4d-gaussian-splatting)]
* A Compact Dynamic 3D Gaussian Representation for Real-Time Dynamic View Synthesis, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2311.12897.pdf)] [[Website](https://compactdynamic3dgaussian.github.io/)] [[Code](https://github.com/raven38/EfficientDynamic3DGaussian)]
* DynMF: Neural Motion Factorization for Real-time Dynamic View Synthesis with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00112.pdf)] [[Website](https://agelosk.github.io/dynmf/)] [[Code](https://github.com/agelosk/dynmf)]
* SC-GS: Sparse-Controlled Gaussian Splatting for Editable Dynamic Scenes, **CVPR, 2024**. [[Paper](https://yihua7.github.io/SC-GS-web/materials/SC_GS_Arxiv.pdf)] [[Website](https://yihua7.github.io/SC-GS-web/)] [[Code](https://github.com/yihua7/SC-GS)]
* Gaussian-Flow: 4D Reconstruction with Dynamic 3D Gaussian Particle, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2310.08528.pdf)] [[Website](https://nju-3dv.github.io/projects/Gaussian-Flow)]
* GauFRe: Gaussian Deformation Fields for Real-time Dynamic Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.11458.pdf)] [[Website](https://lynl7130.github.io/gaufre/index.html)]
* Spacetime Gaussian Feature Splatting for Real-Time Dynamic View Synthesis, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.16812.pdf)] [[Website](https://oppo-us-research.github.io/SpacetimeGaussians-website/)] [[Code](https://github.com/oppo-us-research/SpacetimeGaussians)]
* SWinGS: Sliding Windows for Dynamic 3D Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.13308.pdf)] [[Website](https://arxiv.org/abs/2312.13308)] [[Code](https://github.com/tyhuang0428/DreamPhysics)]
* DreamGaussian4D: Generative 4D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.17142.pdf)] [[Website](https://jiawei-ren.github.io/projects/dreamgaussian4d/)] [[Code](https://github.com/jiawei-ren/dreamgaussian4d)]
* 4DGen: Grounded 4D Content Generation with Spatial-temporal Consistency, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.17225.pdf)] [[Website](https://github.com/VITA-Group/4DGen)] [[Code](https://www.youtube.com/watch?v=-bXyBKdpQ1o)]
* Neural Parametric Gaussians for Monocular Non-Rigid Object Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.01196.pdf)]
* CoGS: Controllable Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.05664.pdf)] [[Website](https://cogs2023.github.io/)]
* MD-Splatting: Learning Metric Deformation from 4D Gaussians in Highly Deformable Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00583)] [[Website](https://md-splatting.github.io/)] [[Code](https://github.com/momentum-robotics-lab/md-splatting)]
* 3DGStream: On-the-Fly Training of 3D Gaussians for Efficient Streaming of Photo-Realistic Free-Viewpoint Videos, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.01444.pdf)] [[Website](https://sjojok.github.io/3dgstream/)] [[Code](https://github.com/SJoJoK/3DGStream)]
* Dynamic Gaussian Splatting from Markerless Motion Capture can Reconstruct Infants Movements, **WACV, 2024**. [[Paper](https://arxiv.org/pdf/2310.19441)]
* GaussianPrediction: Dynamic 3D Gaussian Prediction for Motion Extrapolation and Free View Synthesis, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2405.19745)] [[Website](https://arxiv.org/abs/2405.19745)] [[Code](https://github.com/BoMingZhao/GaussianPrediction)
* VEGS: View Extrapolation of Urban Scenes in 3D Gaussian Splatting using Learned Priors, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.02945)] [[Code](https://github.com/deepshwang/vegs)]
* Neural Parametric Gaussians for Monocular Non-Rigid Object Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2312.01196)]
* Gaussian Splatting LK, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.11309)]
* HDRSplat: Gaussian Splatting for High Dynamic Range 3D Scene Reconstruction from Raw Images, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.16503)]
* Reality Fusion: Robust Real-time Immersive Mobile Robot Teleoperation with Volumetric Visual Data Fusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.01225)]
* HDRGS: High Dynamic Range Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.06543)]
* S4D: Streaming 4D Real-World Reconstruction with Gaussians and 3D Control Points, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.13036)]
* DynOMo: Online Point Tracking by Dynamic Online Monocular Gaussian Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.02104)]
* DENSER: 3D Gaussians Splatting for Scene Reconstruction of Dynamic Urban Environments, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10041)]
* SplatFields: Neural Gaussian Splats for Sparse 3D and 4D Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.11211)]

### Localization & Visual SLAM
* SGS-SLAM: Semantic Gaussian Splatting For Neural Dense SLAM,  **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2402.03246.pdf)]
* Compact 3D Gaussian Splatting For Dense Visual SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.11247.pdf)] [[Code](https://github.com/dtc111111/Compact_GSSLAM)]
* NGM-SLAM: Gaussian Splatting SLAM with Radiance Field Submap, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.05702)]
* GGRt: Towards Generalizable 3D Gaussians without Pose Priors in Real-Time, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10147)] [[Website](https://3d-aigc.github.io/GGRt/)]
* MGS-SLAM: Monocular Sparse Tracking and Gaussian Mapping with Depth Smooth Regularization, *arXiv 2024*. [[Paper](https://arxiv.org/pdf/2405.06241)]
* GS-SLAM: Dense Visual SLAM with 3D Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.11700.pdf)]
* Photo-SLAM: Real-time Simultaneous Localization and Photorealistic Mapping for Monocular, Stereo, and RGB-D Cameras, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.16728.pdf)]
* SplaTAM: Splat, Track & Map 3D Gaussians for Dense RGB-D SLAM, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.02126.pdf)] [[Website](https://spla-tam.github.io/)] [[Code](https://github.com/spla-tam/SplaTAM)]
* Gaussian Splatting SLAM, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.06741.pdf)] [[Code](https://github.com/muskie82/MonoGS)] [[Website](https://rmurai.co.uk/projects/GaussianSplattingSLAM/)]
* Gaussian-SLAM: Photo-realistic Dense SLAM with Gaussian Splatting, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2312.10070.pdf)] [[Code](https://github.com/VladimirYugay/Gaussian-SLAM)] [[Website](https://vladimiryugay.github.io/gaussian_slam/)]
* SemGauss-SLAM: Dense Semantic Gaussian Splatting SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.07494.pdf)]
* NEDS-SLAM: A Novel Neural Explicit Dense Semantic SLAM Framework using 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.11679.pdf)]
* High-Fidelity SLAM Using Gaussian Splatting with Rendering-Guided Densification and Regularized Optimization, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.12535.pdf)]
* RGBD GS-ICP SLAM, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.12550.pdf)] [[Code](https://github.com/Lab-of-AI-and-Robotics/GS_ICP_SLAM)] [[Video](https://www.youtube.com/watch?v=e-bHh_uMMxE)]
* EndoGSLAM: Real-Time Dense Reconstruction and Tracking in Endoscopic Surgeries using Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.15124.pdf)] [[Website](https://endogslam.loping151.com/)] [[Code](https://github.com/Loping151/EndoGSLAM)]
* CG-SLAM: Efficient Dense RGB-D SLAM in a Consistent Uncertainty-aware 3D Gaussian Field, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2403.16095.pdf)] [[Code](https://github.com/hjr37/CG-SLAM)] [[Website](https://zju3dv.github.io/cg-slam/)]
* RTG-SLAM: Real-time 3D Reconstruction at Scale using Gaussian Splatting, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2404.19706)] [[Code](https://github.com/MisEty/RTG-SLAM)]
* MotionGS: Compact Gaussian Splatting SLAM by Motion Filter, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.11129)] [[Code](https://github.com/Antonio521/MotionGS)]
* Monocular Gaussian SLAM with Language Extended Loop Closure, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.13748)]
* Splat-SLAM: Globally Optimized RGB-only SLAM with 3D Gaussians, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.16544)] [[Code](https://github.com/eriksandstroem/Splat-SLAM)]
* MG-SLAM: Structure Gaussian SLAM with Manhattan World Hypothesis, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.20031)]
* TAMBRIDGE: Bridging Frame-Centered Tracking and 3D Gaussian Splatting for Enhanced SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.19614)] [[Code](https://github.com/ZeldaFromHeaven/TAMBRIDGE-DAVID)] [[Website](https://zeldafromheaven.github.io/TAMBRIDGE/)]
* 3DGS-ReLoc: 3D Gaussian Splatting for Map Representation and Visual ReLocalization, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11367)] [[Website](https://arxiv.org/abs/2403.11367)]
* IG-SLAM: Instant Gaussian SLAM, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.01126)]
* Visual SLAM with 3D Gaussian Primitives and Depth Priors Enabling Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.05635)]
* Towards Real-Time Gaussian Splatting: Accelerating 3DGS through Photometric SLAM, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.05635)]
* OG-Mapping: Octree-based Structured 3DGaussians for Online Dense Mapping, *arXiv*. [[Paper](https://arxiv.org/pdf/2408.17223)]
* 3DGS-Calib: 3D Gaussian Splatting for Multimodal SpatioTemporal Calibration, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11577)] [[Website](https://arxiv.org/abs/2403.11577)]
* COLMAP-Free 3D Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.07504.pdf)]
* 6DGS: 6D Pose Estimation from a Single Image and a 3D Gaussian Splatting Model, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2407.15484)] [[Code](https://github.com/mbortolon97/6dgs)]
* Hi-SLAM: Scaling-up Semantics in SLAM with a Hierarchically Categorical Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.12518)]
* GLC-SLAM: Gaussian Splatting SLAM with Efficient Loop Closure, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10982)]
* GSplatLoc: Grounding Keypoint Descriptors into 3D Gaussian Splatting for Improved Visual Localization, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.16502)]
* SplatLoc: 3D Gaussian Splatting-based Visual Localization for Augmented Reality, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.14067)]
* GS-Pose: Cascaded Framework for Generalizable Segmentation-based 6D Object Pose Estimation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10683)] [[Website](https://dingdingcai.github.io/gs-pose/)] [[Code](https://github.com/dingdingcai/GSPose)]
* HGSLoc: 3DGS-based Heuristic Camera Pose Refinement, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10925.pdf)]

### Multimodal-SLAM
* Multi-Modal Neural Radiance Field for Monocular Dense SLAM with a Light-Weight ToF Sensor, **ICCV, 2023**. [[Paper](https://arxiv.org/pdf/2308.14383.pdf)] [[Website](https://zju3dv.github.io/tof_slam/)] [[Code](https://github.com/zju3dv/tof_slam)]
* LIV-GaussMap: LiDAR-Inertial-Visual Fusion for Real-time 3D Radiance Field Map Rendering, **RAL, 2024**. [[Paper](https://arxiv.org/pdf/2401.14857.pdf)] [[Code](https://github.com/sheng00125/LIV-GaussMap)]
* MM3DGS SLAM: Multi-modal 3D Gaussian Splatting for SLAM Using Vision, Depth, and Inertial Measurements, **IROS, 2024**. [[Paper](https://arxiv.org/pdf/2404.00923.pdf)] [[Website](https://vita-group.github.io/MM3DGS-SLAM/)]
* MM-Gaussian: 3D Gaussian-based Multi-modal Fusion for Localization and Reconstruction in Unbounded Scenes, **IROS, 2024**. [[Paper](https://arxiv.org/pdf/2404.04026.pdf)]
* Gaussian-LIC: Photo-realistic LiDAR-Inertial-Camera SLAM with 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.06926.pdf)]
* Go-SLAM: Grounded Object Segmentation and Localization with Gaussian Splatting SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2409.16944.pdf)]



## Planning & Navigation
* Beyond Uncertainty: Risk-Aware Active View Acquisition for Safe Robot Navigation and 3D Scene Understanding with FisherRF, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11396)] [[Website](https://arxiv.org/abs/2403.11396)]
* HO-Gaussian: Hybrid Optimization of 3D Gaussian Splatting for Urban Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20032.pdf)] [[Website](https://arxiv.org/abs/2403.20032)]
* Splat-Nav: Safe Real-Time Robot Navigation in Gaussian Splatting Maps, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.02751.pdf)]
* GaussNav: Gaussian Splatting for Visual Navigation, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.11625.pdf)] [[Code](https://github.com/XiaohanLei/GaussNav)] [[Website](https://xiaohanlei.github.io/projects/GaussNav/)]
* GS-Planner: A Gaussian-Splatting-based Planning Framework for Active High-Fidelity Reconstruction, **IROS, 2024**. [[Paper](https://arxiv.org/pdf/2405.10142)] [[Video](https://www.bilibili.com/video/BV1e1421S7Kh/)]
* Scaling 3D Reasoning with LMMs to Large Robot Mission Environments Using Datagraphs, *arXiv*. [[Paper](https://arxiv.org/abs/2407.10743)]
* DHGS: Decoupled Hybrid Gaussian Splatting for Driving Scene, *arXiv*. [[Paper](https://arxiv.org/abs/2407.16600)]
* Active Implicit Reconstruction Using One-Shot View Planning, **ICRA, 2024**. [[Paper](https://arxiv.org/pdf/2310.00685)]
* BEINGS: Bayesian Embodied Image-goal Navigation with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2409.10216)]
* SAFER-Splat: A Control Barrier Function for Safe Navigation with Online Gaussian Splatting Maps, *arXiv*. [[Paper](https://arxiv.org/abs/2409.09868)]
* RT-GuIDE: Real-Time Gaussian splatting for Information-Driven Exploration, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.18122)]




## Manipulation & RL
* Ditto: Building Digital Twins of Articulated Objects from Interaction, **CVPR, 2022**. [[Paper](https://arxiv.org/abs/2202.08227)] [[Code](https://github.com/UT-Austin-RPL/Ditto)] [[Website](https://ut-austin-rpl.github.io/Ditto/)]
* Relational-NDF:SE(3)-Equivariant Relational Rearrangement with Neural Descriptor Fields, **CoRL 2022**. [[Paper](https://arxiv.org/pdf/2211.09786.pdf)] [[Code](https://github.com/anthonysimeonov/relational_ndf)] [[Website](https://anthonysimeonov.github.io/r-ndf/)]
* Neural Descriptor Fields:SE(3)-Equivariant Object Representations for Manipulation, **ICRA, 2022**. [[Paper](https://arxiv.org/abs/2112.05124)] [[Code](https://github.com/anthonysimeonov/ndf_robot)] [[Website](https://yilundu.github.io/ndf/)]
* Neural Motion Fields: Encoding Grasp Trajectories as Implicit Value Functions, **RSS 2022**. [[Paper](https://arxiv.org/pdf/2206.14854.pdf)]  [[Video](https://youtu.be/B-pEhT1pi-Q)]
* Grasping Field: Learning Implicit Representations for Human Grasps, **3DV 2020**. [[Paper](https://arxiv.org/pdf/2008.04451.pdf)] [[Code](https://github.com/korrawe/grasping_field)] [[Video](https://youtu.be/J8x5i1FCgTQ)]
* GIGA: Synergies Between Affordance and Geometry: 6-DoF Grasp Detection via Implicit Representations, **RSS, 2021**. [[Paper](https://arxiv.org/abs/2104.01542)] [[Code](https://github.com/UT-Austin-RPL/GIGA)] [[Website](https://sites.google.com/view/rpl-giga2021)]
* ObjectFolder: A Dataset of Objects with Implicit Visual, Auditory, and Tactile Representations, **CoRL, 2021**. [[Paper](https://arxiv.org/pdf/2109.07991.pdf)] [[Code](https://github.com/rhgao/ObjectFolder)] [[Website](https://ai.stanford.edu/~rhgao/objectfolder/)]
* ObjectFolder 2.0: A Multisensory Object Dataset for Sim2Real Transfer, **CVPR, 2022**. [[Paper](https://arxiv.org/pdf/2204.02389.pdf)] [[Code](https://github.com/rhgao/ObjectFolder)] [[Website](https://ai.stanford.edu/~rhgao/objectfolder2.0/)]
* Local Neural Descriptor Fields: Locally Conditioned Object Representations for Manipulation, **ICRA, 2023**. [[Paper](https://arxiv.org/pdf/2302.03573.pdf)] [[Code](https://github.com/elchun/lndf_robot)] [[Website](https://elchun.github.io/lndf/)]
* Equivariant Descriptor Fields: SE(3)-Equivariant Energy-Based Models for End-to-End Visual Robotic Manipulation Learning, **ICLR, 2023**. [[Paper](https://openreview.net/forum?id=dnjZSPGmY5O)] [[Code](https://github.com/tomato1mule/edf)]
* Point'n Move: Interactive Scene Object Manipulation on Gaussian Splatting Radiance Fields, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.16737.pdf)]
* MANUS: Markerless Hand-Object Grasp Capture using Articulated 3D Gaussians, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.02137.pdf)]
* Reinforcement Learning with Generalizable Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.07950.pdf)]
* GaussianGrasper: 3D Language Gaussian Splatting for Open-vocabulary Robotic Grasping, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09637)] [[Code](https://github.com/MrSecant/GaussianGrasper)]
* 3D-Aware Manipulation with Object-Centric Gaussian Splatting, *arXiv*. [[Paper](https://object-aware-gaussian.github.io/assets/pdf/corl.pdf)] [[Website](https://object-aware-gaussian.github.io/)]
* Gaussian Splatting to Real World Flight Navigation Transfer with Liquid Networks, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.15149)]
* ManiGaussian: Dynamic Gaussian Splatting for Multi-task Robotic Manipulation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08321)]
* Physically Embodied Gaussian Splatting: A Realtime Correctable World Model for Robotics, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.10788)]
* Radiance Fields for Robotic Teleoperation, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.20194)]
* Dynamic 3D Gaussian Tracking for Graph-Based Neural Dynamics Modeling, *arXiv*. [[Paper](https://gaussian-gbnd.github.io/)]
* GraspSplats: Efficient Manipulation with 3D Feature Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.02084)]
* SplatSim: Zero-Shot Sim2Real Transfer of RGB Manipulation Policies Using Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.10161)]
* HGS-Planner: Hierarchical Planning Framework for Active Scene Reconstruction Using 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2409.17624)]
* DreamHOI: Subject-Driven Generation of 3D Human-Object Interactions with Diffusion Priors, *arXiv*. [[Paper](https://arxiv.org/abs/2409.08279)]

## Simulation & Generation
* Control4D: Efficient 4D Portrait Editing with Text, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2305.20082.pdf)] [[Website](https://control4darxiv.github.io/)]
* Comp4D: LLM-Guided Compositional 4D Scene Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.16993.pdf)] [[Website](https://vita-group.github.io/Comp4D/)] [[Code](https://github.com/VITA-Group/Comp4D)]
* GALA3D: Towards Text-to-3D Complex Scene Generation via Layout-guided Generative Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.07207.pdf)] [[Website](https://gala3d.github.io/)] [[Code](https://github.com/VDIGPKU/GALA3D)]
* Controllable Text-to-3D Generation via Surface-Aligned Gaussian Splatting, *arXiv*. [[Paper](https://lizhiqi49.github.io/MVControl/assets/paper.pdf)] [[Website](https://lizhiqi49.github.io/MVControl/)] [[Code](https://github.com/WU-CVGL/MVControl-threestudio)]
* Hyper-3DG:Text-to-3D Gaussian Generation via Hypergraph, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09236.pdf)] [[Website](https://arxiv.org/abs/2403.09236)] [[Code](https://github.com/yjhboy/Hyper3DG)]
* DreamScene: 3D Gaussian-based Text-to-3D Scene Generation via Formation Pattern Sampling, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.03575.pdf)] [[Website](https://dreamscene-project.github.io/)] [[Code](https://github.com/DreamScene-Project/DreamScene)]
* BrightDreamer: Generic 3D Gaussian Generative Framework for Fast Text-to-3D Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11273)] [[Website](https://vlislab22.github.io/BrightDreamer/)] [[Code](https://github.com/lutao2021/BrightDreamer)]
* GVGEN: Text-to-3D Generation with Volumetric Representation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.12957)] [[Website](https://gvgen.github.io/)] [[Code](https://github.com/GVGEN/GVGEN)]
* DreamPolisher: Towards High-Quality Text-to-3D Generation via Geometric Diffusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.17237)] [[Website](https://yuanze-lin.me/DreamPolisher_page/)] [[Code](https://github.com/yuanze-lin/DreamPolisher)]
* DreamScene360: Unconstrained Text-to-3D Scene Generation with Panoramic Gaussian Splatting, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2404.06903)] [[Website](https://dreamscene360.github.io/)]
* RealmDreamer: Text-Driven 3D Scene Generation with Inpainting and Depth Diffusion, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.07199)] [[Website](https://realmdreamer.github.io/)]
* Text-to-3D using Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2309.16585.pdf)] [[Website](https://gsgen3d.github.io/)] [[Code](https://github.com/gsgen3d/gsgen)]
* DreamGaussian: Generative Gaussian Splatting for Efficient 3D Content Creation, *arXiv*. [[Paper](https://arxiv.org/pdf/2309.16653.pdf)] [[Website](https://dreamgaussian.github.io/)] [[Code](https://github.com/dreamgaussian/dreamgaussian)]
* GaussianDreamer: Fast Generation from Text to 3D Gaussian Splatting with Point Cloud Priors, *arXiv*. [[Paper](https://arxiv.org/pdf/2310.08529.pdf)] [[Website](https://taoranyi.com/gaussiandreamer/)] [[Code](https://github.com/hustvl/GaussianDreamer)]
* GaussianDiffusion: 3D Gaussian Splatting for Denoising Diffusion Probabilistic Models with Structured Noise, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.11221.pdf)] [[Website](https://arxiv.org/abs/2311.11221)]
* LucidDreamer: Towards High-Fidelity Text-to-3D Generation via Interval Score Matching, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.11284.pdf)] [[Website](https://arxiv.org/abs/2311.11284)] [[Code](https://github.com/EnVision-Research/LucidDreamer)]
* CG3D: Compositional Generation for Text-to-3D, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.17907.pdf)] [[Website](https://asvilesov.github.io/CG3D/)]
* Align Your Gaussians: Text-to-4D with Dynamic 3D Gaussians and Composed Diffusion Models, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2304.08818.pdf)] [[Website](https://research.nvidia.com/labs/toronto-ai/AlignYourGaussians/)]
* Text2Immersion: Generative Immersive Scene with 3D Gaussian, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.09242.pdf)] [[Website](https://ken-ouyang.github.io/text2immersion/index.html)]
* GSEdit: Efficient Text-Guided Editing of 3D Objects via Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.05154.pdf)]
* GaussCtrl: Multi-View Consistent Text-Driven 3D Gaussian Splatting Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08733.pdf)]
* View-Consistent 3D Editing with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11868.pdf)]
* Gaussian Frosting: Editable Complex Radiance Fields with Real-Time Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14554)] [[Website](https://anttwo.github.io/frosting/)] [[Code](https://github.com/Anttwo/Frosting)]
* ICE-G: Image Conditional Editing of 3D Gaussian Splats, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2406.08488)] [[Website](https://ice-gaussian.github.io/)]
* GaussianEditor: Swift and Controllable 3D Editing with Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.14521.pdf)] [[Website](https://buaacyw.github.io/gaussian-editor/)] [[Code](https://github.com/buaacyw/GaussianEditor)]
* GaussianEditor: Editing 3D Gaussians Delicately with Text Instructions, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.16037.pdf)] [[Website](https://gaussianeditor.github.io/)]
* Gaussian Grouping: Segment and Edit Anything in 3D Scenes, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.00732.pdf)] [[Code](https://github.com/lkeab/gaussian-grouping)]
* StyleGaussian: Instant 3D Style Transfer with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.07807.pdf)] [[Website](https://kunhao-liu.github.io/StyleGaussian/)] [[Code](https://github.com/Kunhao-Liu/StyleGaussian)]
* Gaussian Splatting in Style, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08498)]
* StylizedGS: Controllable Stylization for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.05220)]
* 3DEgo: 3D Editing on the Go!, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.10102.pdf)]
* GScream: Learning 3D Geometry and Feature Consistent Gaussian Splatting for Object Removal, **ECCV, 2024**. [[Paper](https://arxiv.org/abs/2404.13679)]
* Gaussian Splatting with Localized Points Management, *arXiv, 2024*. [[Paper](https://arxiv.org/abs/2406.04251)]
* Localized Gaussian Splatting Editing with Contextual Awareness, *arXiv, 2024*. [[Paper](https://arxiv.org/abs/2408.00083)]
* 3D Gaussian Editing with A Single Image, *arXiv*. [[Paper](https://arxiv.org/abs/2408.07540)]
* G-Style: Stylized Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2408.15695)]
* AGG: Amortized Generative 3D Gaussians for Single Image to 3D, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.04099.pdf)] [[Website](https://ir1d.github.io/AGG/)]
* Repaint123: Fast and High-quality One Image to 3D Generation with Progressive Controllable 2D Repainting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.13271.pdf)] [[Website](https://pku-yuangroup.github.io/repaint123/)] [[Coda](https://github.com/PKU-YuanGroup/repaint123)]
* GaussianPU: A Hybrid 2D-3D Upsampling Framework for Enhancing Color Point Clouds via 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2409.01581)]
* WaSt-3D: Wasserstein-2 Distance for Scene-to-Scene Stylization on 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/abs/2409.17917)]
* Generative Object Insertion in Gaussian Splatting with a Multi-View Diffusion Model, *arXiv*. [[Paper](https://arxiv.org/abs/2409.16938)]
* TIP-Editor: An Accurate 3D Editor Following Both Text-Prompts And Image-Prompts, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.14828.pdf)] [[Website](https://zjy526223908.github.io/TIP-Editor/)]
* DreamScene4D: Dynamic Multi-Object Scene Generation from Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.02280)] [[Website](https://dreamscene4d.github.io/)] [[Code](https://github.com/dreamscene4d/dreamscene4d)]
* Connecting Consistency Distillation to Score Distillation for Text-to-3D Generation, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2407.13584)] [[Code](https://github.com/LMozart/ECCV2024-GCS-BEG)]
* DreamMapping: High-Fidelity Text-to-3D Generation via Variational Distribution Mapping, *arXiv*. [[Paper](https://arxiv.org/abs/2409.05099)]
* DreamMesh: Jointly Manipulating and Texturing Triangle Meshes for Text-to-3D Generation, *arXiv*. [[Paper](https://arxiv.org/abs/2409.07454)]
* Hi3D: Pursuing High-Resolution Image-to-3D Generation with Video Diffusion Models, *arXiv*. [[Paper](https://arxiv.org/abs/2409.07452)]
* SceneTeller: Language-to-3D Scene Generation, **ECCV 2024**. [[Paper](https://arxiv.org/pdf/2407.20727.pdf)]
* HoloDreamer: Holistic 3D Panoramic World Generation from Text Descriptions, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.15187.pdf)]
* SV4D: Dynamic 3D Content Generation with Multi-Frame and Multi-View Consistency, *arXiv*. [[Paper](https://arxiv.org/pdf/2407.17470.pdf)]
* ART3D: 3D Gaussian Splatting for Text-Guided Artistic Scenes Generation, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2405.10508.pdf)]

---
## Citation

If you find this repository useful, please consider citing this list:

```
@misc{Deng20243dgspaperlist,
    title = {awesome-Implicit-NeRF-SLAM},
    author = {Tianchen Deng, Yue Pan, Xingxing Zuo, Shenghai Yuan, Nailin Wang, Hesheng Wang, Jingchuan Wang, Cyrill Stachniss, Lihua Xie, Danwei Wang, Weidong Chen},
    howpublished = {\url{https://github.com/dtc111111/awesome-3dgs-for-robotics}},
    year = {2024}
}
```

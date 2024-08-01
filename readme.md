<div align="center">    
<img src="Images/image1.png" width="600" height="480" />   

# Awesome 3D Gaussian Splatting for Robotics [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This repo contains a curative list of **3D Gaussian Splatting papers relating to the Robotics domain**.

#### Please feel free to send me [pull requests](https://github.com/dtc111111/awesome-3dgs-for-robotics) or [email](mailto:dengtianchen@sjtu.edu.cn) to add papers! <br>

If you find this repository useful, please consider [citing](#citation) and STARing this list. Feel free to share this list with others!

---

## Overview
  - [3DGS Survey](#3dgs-survey)
    
  - [3DGS Foundation Model](#3dgs-general-model)
    - [Sparse View](#sparseview)
    - [Accelerate & Compression](#acccompression)
    - [Physics](#physics)

  - [Perception](#perception)
    - [Semantic](#Semantic)
    - [Multi-Modal](#MM)
    - [Object Detection](#Object-Detection)
    - [Relightable & Complex Environment & Rainy](#Relightable)
    
  - [Mapping & Localization](#slam)
    - [3D Reconstruction](#3D-Reconstruction)
    - [Dynamic Scene Reconstruction](#Dynamic-Reconstruction)
    - [Localization & Visual SLAM](#Visual-SLAM)
    - [Multimodal-SLAM](#Multimodal-SLAM)
      
  - [Planning & Navigation](#planningnavigation)
  - [Manipulation & RL](#manipulationrl)
  - [Simulation & Human Interaction](#editing)

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

## 3DGS Foundation Model
---
* 3D Gaussian Splatting for Real-Time Radiance Field Rendering, **SIGGRAPH, 2023**. [[Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf)] [[Website](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)]
* 2D Gaussian Splatting for Geometrically Accurate Radiance Fields, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2403.17888)] [[Website](https://surfsplatting.github.io/)]  [[Code](https://github.com/hbb1/2d-gaussian-splatting)]
* Mip-splatting: Alias-free 3d gaussian splatting, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_Mip-Splatting_Alias-free_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)] [[Website](https://niujinshuchong.github.io/mip-splatting/)]  [[Code](https://github.com/autonomousvision/mip-splatting)]
* End-to-End Rate-Distortion Optimized 3D Gaussian Representation, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2406.01597.pdf)] [[Website](https://arxiv.org/abs/2406.01597)] [[Code](https://github.com/USTC-IMCL/RDO-Gaussian)]
  
### Sparse View
* AGG: Amortized Generative 3D Gaussians for Single Image to 3D, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.04099.pdf)] [[Website](https://ir1d.github.io/AGG/)]
* Fast Dynamic 3D Object Generation from a Single-view Video, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.08742.pdf)] [[Website](https://fudan-zvg.github.io/Efficient4D/)] [[Code](https://github.com/fudan-zvg/Efficient4D)]
* GaussianObject: Just Taking Four Images to Get A High-Quality 3D Object with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.10259.pdf)] [[Website](https://gaussianobject.github.io/)] [[Code](https://github.com/GaussianObject/GaussianObject)]
* LGM: Large Multi-View Gaussian Model for High-Resolution 3D Content Creation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.05054.pdf)] [[Website](https://me.kiui.moe/lgm/)] [[Code](https://github.com/3DTopia/LGM)]
* IM-3D: Iterative Multiview Diffusion and Reconstruction for High-Quality 3D Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.08682.pdf)] [[Website](https://arxiv.org/abs/2402.08682)]
* FDGaussian: Fast Gaussian Splatting from Single Image via Geometric-aware Diffusion Model, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10242.pdf)] [[Website](https://qjfeng.net/FDGaussian)]
* Repaint123: Fast and High-quality One Image to 3D Generation with Progressive Controllable 2D Repainting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.13271.pdf)] [[Website](https://pku-yuangroup.github.io/repaint123/)] [[Coda](https://github.com/PKU-YuanGroup/repaint123)]
* Depth-Regularized Optimization for 3D Gaussian Splatting in Few-Shot Images, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.13398.pdf)] [[Website](https://robot0321.github.io/DepthRegGS/index.html)] [[Coda](https://github.com/robot0321/DepthRegularizedGS)]


### Accelerate & Compression
* Hash3D: Training-free Acceleration for 3D Generation, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.06091)] [[Website](https://adamdad.github.io/hash3D/)] [[Code](https://github.com/Adamdad/hash3D)]
* Characterizing Satellite Geometry via Accelerated 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.02588.pdf)]
* TRIPS: Trilinear Point Splatting for Real-Time Radiance Field Renderin, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.06003.pdf)] [[Website](https://lfranke.github.io/trips/)] [[Code](https://github.com/lfranke/trips)]
* LIV-GaussMap: LiDAR-Inertial-Visual Fusion for Real-time 3D Radiance Field Map Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.14857.pdf)] [[Code](https://github.com/sheng00125/LIV-GaussMap)]
* Splat-Nav: Safe Real-Time Robot Navigation in Gaussian Splatting Maps, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.02751.pdf)]
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
* GaussianPro: 3D Gaussian Splatting with Progressive Propagation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.14650.pdf)] [[Website](https://kcheng1021.github.io/gaussianpro.github.io/)] [[Code](https://github.com/kcheng1021/GaussianPro)]
* 





### Physics
* Gaussian Splashing: Dynamic Fluid Synthesis with Gaussian Splatting, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2401.15318.pdf)] [[Website](https://amysteriouscat.github.io/GaussianSplashing/)]
* GaMeS: Mesh-Based Adapting and Modification of Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.01459.pdf)] [[Code](https://github.com/waczjoan/gaussian-mesh-splatting)]
* Mesh-based Gaussian Splatting for Real-time Large-scale Deformation, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.04796.pdf)]
* Reconstruction and Simulation of Elastic Objects with Spring-Mass 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09434)] [[Website](https://zlicheng.com/spring_gaus/)] [[Code](https://github.com/Colmar-zlicheng/Spring-Gaus)]
* Texture-GS: Disentangling the Geometry and Texture for 3D Gaussian Splatting Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10050)] [[Website](https://slothfulxtx.github.io/TexGS/)] [[Code](https://github.com/slothfulxtx/Texture-GS)]
* DN-Splatter: Depth and Normal Priors for Gaussian Splatting and Meshing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.17822)] [[Website](https://maturk.github.io/dn-splatter/)] [[Code](https://github.com/maturk/dn-splatter)]
* Feature Splatting: Language-Driven Physics-Based Scene Synthesis and Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.01223)] [[Website](https://feature-splatting.github.io/)] [[Code](https://github.com/vuer-ai/feature_splatting)]
* Surface Reconstruction from Gaussian Splatting via Novel Stereo Views, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.01810)] [[Website](https://gs2mesh.github.io/)]
* RaDe-GS: Rasterizing Depth in Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2406.01467)] [[Website](https://baowenz.github.io/radegs/)]
* Trim 3D Gaussian Splatting for Accurate Geometry Representation, *arXiv*. [[Paper](https://arxiv.org/abs/2406.07499)] [[Website](https://trimgs.github.io/)] [[Code](https://github.com/YuxueYang1204/TrimGS)]
* Effective Rank Analysis and Regularization for Enhanced 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/abs/2406.11672)] [[Website](https://junhahyung.github.io/erankgs.github.io/)]
* PhysGaussian: Physics-Integrated 3D Gaussians for Generative Dynamics, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.12198.pdf)] [[Website](https://xpandora.github.io/PhysGaussian/)] [[Code](https://github.com/XPandora/PhysGaussian)]
* SuGaR: Surface-Aligned Gaussian Splatting for Efficient 3D Mesh Reconstruction and High-Quality Mesh Rendering, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.12775.pdf)] [[Website](https://imagine.enpc.fr/~guedona/sugar/)] [[Code](https://github.com/Anttwo/SuGaR)]
* NeuSG: Neural Implicit Surface Reconstruction with 3D Gaussian Splatting Guidance, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00846.pdf)]




## Perception
### Semantic
* Semantic Gaussians: Open-Vocabulary Scene Understanding with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.15624)] [[Website
](https://semantic-gaussians.github.io/)]
* Segment Any 3D Gaussians, *arXiv*. [[Paper](https://jumpat.github.io/SAGA/SAGA_paper.pdf)] [[Website](https://jumpat.github.io/SAGA/)] [[Code](https://github.com/Jumpat/SegAnyGAussians)]
* 2D-Guided 3D Gaussian Segmentation, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.16047.pdf)]

### Multi-Modal
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
* Language Embedded 3D Gaussians for Open-Vocabulary Scene Understanding, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.18482.pdf)] [[Website](https://buaavrcg.github.io/LEGaussians/)] [[Code](https://github.com/buaavrcg/LEGaussians)]
* Feature 3DGS: Supercharging 3D Gaussian Splatting to Enable Distilled Feature Fields, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.03203.pdf)] [[Website](https://feature-3dgs.github.io/)] [[Code](https://github.com/ShijieZhou-UCLA/feature-3dgs)]
* LangSplat: 3D Language Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2312.16084.pdf)] [[Website](https://langsplat.github.io/)] [[Code](https://github.com/minghanqin/LangSplat)]
* FMGS: Foundation Model Embedded 3D Gaussian Splatting for Holistic 3D Scene Understanding, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.01970.pdf)]
* GaussianGrasper: 3D Language Gaussian Splatting for Open-vocabulary Robotic Grasping, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09637)] [[Code](https://github.com/MrSecant/GaussianGrasper)]

### Relightable & Complex Environment & Rainy
* DarkGS: Learning Neural Illumination and 3D Gaussians Relighting for Robotic Exploration in the Dark, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.10814)] [[Code](https://github.com/tyz1030/darkgs)]
* RAIN-GS: Relaxing Accurate Initialization Constraint for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.09413)] [[Website](https://ku-cvlab.github.io/RAIN-GS/)] [[Code](https://github.com/KU-CVLAB/RAIN-GS)]
* Gaussian Shadow Casting for Neural Characters, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2401.06116.pdf)]
  

## Mapping & Localization
### 3D Reconstruction
* VastGaussian: Vast 3D Gaussians for Large Scene Reconstruction, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2402.17427.pdf)] [[Website](https://vastgaussian.github.io/)] [[Code](https://github.com/kangpeilun/VastGaussian)]
* Spec-Gaussian: Anisotropic View-Dependent Appearance for 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.15870.pdf)]
  

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
* Per-Gaussian Embedding-Based Deformation for Deformable 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.03613)] [[Website](https://jeongminb.github.io/e-d3dgs/)] [[Code](https://github.com/JeongminB/E-D3DGS)]
* DreamScene4D: Dynamic Multi-Object Scene Generation from Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.02280)] [[Website](https://dreamscene4d.github.io/)] [[Code](https://github.com/dreamscene4d/dreamscene4d)]
* 3D Geometry-aware Deformable Gaussian Splatting for Dynamic View Synthesis, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2404.06270)] [[Website](https://npucvr.github.io/GaGS/)]
* Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis, *3DV, 2024*. [[Paper](https://dynamic3dgaussians.github.io/paper.pdf)] [[Website](https://dynamic3dgaussians.github.io/)] [[Code](https://github.com/JonathonLuiten/Dynamic3DGaussians)]
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
* 



### Visual-SLAM
* **NeuralRecon**: Real-Time Coherent 3D Reconstruction from Monocular Video, *CVPR, 2021*.[[Paper](https://arxiv.org/pdf/2104.00681.pdf)] [[Pytorch Code](https://github.com/zju3dv/NeuralRecon/)] [[Website](https://zju3dv.github.io/neuralrecon/)]
* **Di-fusion**: Online implicit 3d reconstruction with deep priors, *CVPR, 2021*.[[Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Huang_DI-Fusion_Online_Implicit_3D_Reconstruction_With_Deep_Priors_CVPR_2021_paper.pdf)] [[Pytorch Code](https://github.com/huangjh-pub/di-fusion)] 
* **iSDF**: Real-Time Neural Signed Distance Fields for Robot Perception, *RSS, 2022*. [[Paper](https://arxiv.org/abs/2204.02296)] [[Pytorch Code](https://github.com/facebookresearch/iSDF)] [[Website](https://joeaortiz.github.io/iSDF/)]
* **LENS**: LENS: Localization enhanced by NeRF synthesis, *CoRL, 2021*. [[Paper](https://arxiv.org/abs/2110.06558)] [[Video](https://www.youtube.com/watch?v=DgIpVoS6ejY)] 
* **NICE-SLAM**: Neural Implicit Scalable Encoding for SLAM, *CVPR, 2021*. [[Paper](https://arxiv.org/abs/2112.12130)] [[Pytorch Code](https://github.com/cvg/nice-slam)] [[Website](https://pengsongyou.github.io/nice-slam?utm_source=catalyzex.com)]
* **iMAP**: Implicit Mapping and Positioning in Real-Time, *ICCV, 2021*. [[Paper](https://arxiv.org/abs/2103.12352)] [[Website](https://edgarsucar.github.io/iMAP/)] [[Video](https://www.youtube.com/watch?v=c-zkKGArl5Y)] 
* **BNV-Fusion**: BNV-Fusion: Dense 3D Reconstruction using Bi-level Neural Volume Fusion, *CVPR, 2022*. [[Paper](https://arxiv.org/pdf/2204.01139.pdf)] [[Pytorch Code](https://github.com/likojack/bnv_fusion)]
* **NeRF-SLAM**: Real-Time Dense Monocular SLAM with Neural Radiance Fields, *IROS, 2023*. [[Paper](https://arxiv.org/pdf/2210.13641.pdf)] [[Pytorch Code](https://github.com/ToniRV/NeRF-SLAM)] [[Video](https://www.youtube.com/watch?v=-6ufRJugcEU)]
* **Nerfels**: Renderable Neural Codes for Improved Camera Pose Estimation, *CVPR 2022 Workshop*. [[Paper](https://openaccess.thecvf.com/content/CVPR2022W/IMW/papers/Avraham_Nerfels_Renderable_Neural_Codes_for_Improved_Camera_Pose_Estimation_CVPRW_2022_paper.pdf)]
* SDF-based RGB-D Camera Tracking in Neural Scene Representations, *ICRA Workshop, 2022*. [[Paper](https://neural-implicit-workshop.stanford.edu/assets/pdf/bruns.pdf)]
* **Orbeez-SLAM**: A Real-time Monocular Visual SLAM with ORB Features and NeRF-realized Mapping, *ICRA, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10160950)] [[Video](https://www.youtube.com/watch?v=uzb-tVcPETE)] [[Code](https://github.com/MarvinChung/Orbeez-SLAM)]
* **ESLAM**: Efficient Dense SLAM System Based on Hybrid Representation of Signed Distance Fields, *CVPR,  2023*. [[Paper](https://arxiv.org/pdf/2211.11704.pdf)]
* **Vox-Fusion**: Dense Tracking and Mapping with Voxel-based Neural Implicit Representation, *ISMAR,  2022*. [[Paper](https://arxiv.org/pdf/2210.15858.pdf)] [[Website](https://yangxingrui.com/vox-fusion/)] [[Pytorch Code](https://github.com/zju3dv/Vox-Fusion)] [[Video](https://www.youtube.com/watch?v=Prp28y1b2Qs)]
* Visual-Inertial Odometry Priors for Bundle-Adjusting Neural Radiance Fields, *ICCAS, 2022*. [[Paper](http://mpil.sookmyung.ac.kr/wp-content/uploads/2022/12/2022_ICCAS_Kim.pdf)]
* Feature-Realistic Neural Fusion for Real-Time, Open Set Scene Understanding, *ICRA,  2022*. [[Paper](https://arxiv.org/pdf/2210.03043.pdf)]  [[Website](https://yangxingrui.com/vox-fusion/)] [[Video](https://www.youtube.com/watch?v=ysaohKI_Pf0)]
* Towards Open World NeRF-Based SLAM, *CRV, 2023*.  [[Paper](https://arxiv.org/pdf/2301.03102.pdf)]
* Dense RGB SLAM with Neural Implicit Maps, *ICLR, 2023*. [[Paper](https://arxiv.org/pdf/2301.08930v1.pdf)] [[Website](https://poptree.github.io/DIM-SLAM/)] [[Code](https://github.com/HKUST-3DV/DIM-SLAM)] [[Video]()]
* **vMAP**: Vectorised Object Mapping for Neural Field SLAM, *CVPR,  2023*. [[Paper](https://arxiv.org/pdf/2302.01838.pdf)] [[Website](https://kxhit.github.io/vMAP)] [[Pytorch Code](https://github.com/kxhit/vMAP)] [[Video](https://kxhit.github.io/media/vMAP/vmap_raw.mp4)]
* **NICER-SLAM**: Neural Implicit Scene Encoding for RGB SLAM, *3DV 2024*. [[Paper](https://arxiv.org/pdf/2302.03594.pdf)] [[Video](https://www.youtube.com/watch?v=tUXzqEZWg2w)]
* Implicit Map Augmentation for Relocalization, *ECCV Workshop, 2022*. [[Paper](https://link.springer.com/chapter/10.1007/978-3-031-25066-8_36)]
* **Uni-Fusion**: Universal Continuous Mapping, *TRO, 2023*.[[Paper](https://arxiv.org/pdf/2303.12678.pdf)] [[Code](https://github.com/Jarrome/Uni-Fusion)] [[Website](https://jarrome.github.io/Uni-Fusion/)]
* **NEWTON**: Neural View-Centric Mapping for On-the-Fly Large-Scale SLAM, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2303.13654v1.pdf)]
* **Point-SLAM**: Dense Neural Point Cloud-based SLAM, *ICCV, 2023*. [[Paper](https://arxiv.org/pdf/2304.04278.pdf)] [[Code](https://github.com/tfy14esa/Point-SLAM)]
* **RO-MAP**: Real-Time Multi-Object Mapping with Neural Radiance Fields, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/document/10209177)] [[Code](https://github.com/XiaoHan-Git/RO-MAP)] [[Video](https://www.youtube.com/watch?v=sFrLXPw40wU)]
* **Co-SLAM**: Joint Coordinate and Sparse Parametric Encodings for Neural Real-Time SLAM, *CVPR, 2023*. [[Paper](https://arxiv.org/pdf/2304.14377.pdf)] [[Website](https://hengyiwang.github.io/projects/CoSLAM)]
* Neural Implicit Dense Semantic SLAM, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2304.14560.pdf)] [[Code](https://github.com/Yasaman-Haghighi/NeuralImplicitDenseSemanticSLAM)]
* **FMapping**: Factorized Efficient Neural Field Mapping for Real-Time Dense RGB SLAM, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2306.00579v1.pdf)] [[Website](https://vlis2022.github.io/fmap/)] [[Code](https://github.com/thua919/FMapping)] 
* **UncLe-SLAM**: Uncertainty Learning for Dense Neural SLAM, *ICCVw, 2023*. [[Paper](https://arxiv.org/pdf/2306.11048.pdf)] [[Code](https://github.com/kev-in-ta/UncLe-SLAM)]
* **iMODE**:Real-Time Incremental Monocular Dense Mapping Using Neural Field, *ICRA, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10161538)]
* **NISB-Map**: Scalable Mapping With Neural Implicit Spatial Block, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10163242)]
* RGB-D Mapping and Tracking in a Plenoxel Radiance Field, *WACV, 2024*. [[Paper](https://arxiv.org/pdf/2307.03404.pdf)]
* Efficient Map Fusion for Multiple Implicit SLAM Agents, *TIV, 2023*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10189088)]
* **MIPS-Fusion**: Multi-Implicit-Submaps for Scalable and Robust Online Neural RGB-D Reconstruction, *TOG, 2023*. [[Paper](https://arxiv.org/pdf/2308.08741.pdf)]
* **GO-SLAM**: Global Optimization for Consistent 3D Instant Reconstruction, *ICCV, 2023*. [[Paper](https://arxiv.org/pdf/2309.02436.pdf)] [[Website](https://youmi-zym.github.io/projects/GO-SLAM/)] [[Code](https://github.com/youmi-zym/GO-SLAM)] 
* End-to-End RGB-D SLAM with Multi-MLPs Dense Neural Implicit Representations, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10238793)]
* **DynaMoN**: Motion-Aware Fast And Robust Camera Localization for Dynamic NeRF, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2309.08927.pdf)]
* **HI-SLAM**: Monocular Real-time Dense Mapping with Hybrid Implicit Fields, *RAL, 2023*. [[Paper](https://arxiv.org/pdf/2310.04787.pdf)]
* **CP-SLAM**: Collaborative Neural Point-based SLAM, *NeurIPS, 2024*. [[Paper](https://openreview.net/pdf?id=dFSeZm6dTC)] [[Code](https://github.com/hjr37/CP-SLAM)]
* Learning Neural Implicit through Volume Rendering with Attentive Depth Fusion Priors,  *NeurIPS, 2023*. [[Paper](https://arxiv.org/pdf/2310.11598.pdf)] [[Code](https://github.com/MachinePerceptionLab/Attentive_DFPrior)] [[Website](https://machineperceptionlab.github.io/Attentive_DF_Prior/)]
* **NGEL-SLAM**: Neural Implicit Representation-based Global Consistent Low-Latency SLAM System, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2311.09525.pdf)] [[Code](https://github.com/YunxuanMao/ngel_slam)] 
* **SNI-SLAM**: Semantic Neural Implicit SLAM, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2311.11016.pdf)] [[Code](https://github.com/IRMVLab/SNI-SLAM)]
* Implicit Event-RGBD Neural SLAM, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2311.11013.pdf)]
* **DNS SLAM**: Dense Neural Semantic-Informed SLAM, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2312.00204.pdf)]
* **PLGSLAM**: Progressive Neural Scene Represenation with Local to Global Bundle Adjustment, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2312.09866.pdf)]
* **NeRF-VO**: Real-Time Sparse Visual Odometry with Neural Radiance Fields, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2312.13471.pdf)]
* Ternary-type Opacity and Hybrid Odometry for RGB-only NeRF-SLAM, *arXiv, 2023*. [[Paper](https://arxiv.org/pdf/2312.13332.pdf)]
* **DN-SLAM**: A Visual SLAM with ORB Features and NeRF Mapping in Dynamic Environments, *Sensors, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10376402)]
* **NID-SLAM**: Neural Implicit Representation-based RGB-D SLAM in dynamic environments, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2401.01189.pdf)]
* **DDN-SLAM**: Real-time Dense Dynamic Neural Implicit SLAM with Joint Semantic Encoding, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2401.01545.pdf)] [[Code](https://github.com/DrLi-Ming/DDN-SLAM)]
* **Hi-Map**: Hierarchical Factorized Radiance Field for High-Fidelity Monocular Dense Mapping, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2401.03203.pdf)] [[Website](https://vlis2022.github.io/fmap/)] [[Code](https://github.com/thua919/FMapping)]
* **NeuV-SLAM**: Fast Neural Multiresolution Voxel Optimization for RGBD Dense SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2402.02020.pdf)] [[Code](https://github.com/DARYL-GWZ/NeuV-SLAM)]
* **Structerf-SLAM**: Neural implicit representation SLAM for structural environments, *Computers & Graphics, 2024*. [[Paper](https://www.sciencedirect.com/science/article/abs/pii/S0097849324000207)]
* **Loopy-SLAM**: Dense Neural SLAM with Loop Closures, *CVPR, 2024*. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Liso_Loopy-SLAM_Dense_Neural_SLAM_with_Loop_Closures_CVPR_2024_paper.pdf)] [[Code](https://github.com/eriksandstroem/Loopy-SLAM)] [[Website](https://notchla.github.io/Loopy-SLAM/)]
* **Q-SLAM**: Quadric Representations for Monocular SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.08125.pdf)]
* **DVN-SLAM**: Dynamic Visual Neural SLAM Based on Local-Global Encoding, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.11776.pdf)]
* **H3-Mapping**: Quasi-Heterogeneous Feature Grids for Real-time Dense Mapping Using Hierarchical Hybrid Representation, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2403.10821.pdf)] [[Code](https://github.com/SYSU-STAR/H3-Mapping)]
* **Vox-Fusion++**: Voxel-based Neural Implicit Dense Tracking and Mapping with Multi-maps, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.12536.pdf)] [[Code](https://github.com/zju3dv/Vox-Fusion_Plus_Plus)]
* **MUTE-SLAM**: Real-Time Neural SLAM with Multiple Tri-Plane Hash Representations, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.17765.pdf)]
* **GlORIE-SLAM**: Globally Optimized RGB-only Implicit Encoding Point Cloud SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.19549.pdf)] [[Code](https://github.com/zhangganlin/GlORIE-SLAM)] [[Website](https://ganlinzhang.xyz/GlORIE-SLAM/)]
* Efficient 3D Instance Mapping and Localization with Neural Fields, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2403.19797.pdf)] [[Website](https://gtangg12.github.io/iML/)]
* **NeSLAM**: Neural Implicit Mapping and Self-Supervised Feature Tracking With Depth Completion and Denoising, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.20034.pdf)] [[Code](https://github.com/dtc111111/NeSLAM)]
* **KN-SLAM**: Keypoints and Neural Implicit Encoding SLAM, *TIM, 2024*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10474286)]
* **SLAIM**: Robust Dense Neural SLAM for Online Tracking and Mapping, *CVPRw, 2024*. [[Paper](https://arxiv.org/pdf/2404.11419.pdf)] [[Code](https://github.com/vincentcartillier/SLAIM/)] [[Website](https://vincentcartillier.github.io/slaim.html)]
* **EC-SLAM**: Real-time Dense Neural RGB-D SLAM System with Effectively Constrained Global Bundle Adjustment, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.13346.pdf)] [[Code](https://github.com/Lightingooo/EC-SLAM)]
* **S3-SLAM**: Sparse Tri-plane Encoding for Neural Implicit SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.18284)]
* **DF-SLAM**: Neural Feature Rendering Based on Dictionary Factors Representation for High-Fidelity Dense Visual SLAM System, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.17876)] [[Code](https://github.com/funcdecl/DF-SLAM)]
* Neural Graph Mapping for Dense SLAM with Efficient Loop Closure, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.03633)] [[Code](https://github.com/KTH-RPL/neural_graph_mapping)] [[Website](https://kth-rpl.github.io/neural_graph_mapping/)]
* **MGS-SLAM**: Monocular Sparse Tracking and Gaussian Mapping with Depth Smooth Regularization, *arXiv 2024*. [[Paper](https://arxiv.org/pdf/2405.06241)]
* **VPE-SLAM**: Neural Implicit Voxel-Permutohedral Encoding for SLAM, *ICRA, 2024*. [[Paper](todo)] [[Code](https://github.com/NeuCV-IRMI/VPE-SLAM)]
* **ONeK-SLAM**: A Robust Object-Level Dense SLAM Based on Joint Neural Radiance Fields and Keypoints, *ICRA 2024*. [[Paper](todo)]
* **HERO-SLAM**: Hybrid Enhanced Robust Optimization of Neural SLAM, *ICRA, 2024*. [[Paper](todo)] [[Code](https://github.com/hero-slam/HERO-SLAM)] [[Website](https://hero-slam.github.io/)]
* **NeB-SLAM**: Neural Blocks-based Salable RGB-D SLAM for Unknown Scenes, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.15151)]
* **ENeRF-SLAM**:A Dense Endoscopic SLAM With Neural Implicit Representation, *TMRB, 2024*. [[Paper](https://ieeexplore.ieee.org/abstract/document/10542414)] [[Code](https://github.com/Mar-lll/ENeRF-SLAM)]
* IBD-SLAM: Learning Image-Based Depth Fusion for Generalizable SLAM, *CVPR, 2024*. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Yin_IBD-SLAM_Learning_Image-Based_Depth_Fusion_for_Generalizable_SLAM_CVPR_2024_paper.pdf)] [[Website](https://visual-ai.github.io/ibd-slam)]
* **RoDyn-SLAM**: Robust Dynamic Dense RGB-D SLAM with Neural Radiance Fields, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2407.01303)] [[Code](https://github.com/fudan-zvg/Rodyn-SLAM)]
* **MoD-SLAM**: Monocular Dense Mapping for Unbounded 3D Scene Reconstruction,  *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2402.03762.pdf)]
* Evaluating geometric accuracy of NeRF reconstructions compared to SLAM method,  *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2407.11238)]
* **I2-SLAM**: Inverting Imaging Process for Robust Photorealistic Dense SLAM,  *ECCV, 2024*. [[Paper](https://arxiv.org/abs/2407.11347v1)]
* An Artificial-Intelligence-based SLAM Processor with Scene-adaptive Sampling and Hybrid NeRF Model Training Acceleration,  *TCASAI, 2024*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=10595406)]

### Lidar-SLAM
* **SHINE-Mapping**: Large-Scale 3D Mapping Using Sparse Hierarchical Implicit Neural Representations, *ICRA, 2022*. [[Paper](https://arxiv.org/pdf/2210.02299.pdf)] [[Code](https://github.com/PRBonn/SHINE_mapping)]
* **IR-MCL**: Implicit Representation-based Online Global Localization, *RAL, 2023*. [[Paper](https://arxiv.org/pdf/2210.03113.pdf)] [[Code](https://github.com/PRBonn/ir-mcl)]
* Efficient Implicit Neural Reconstruction Using LiDAR, *ICRA, 2023*. [[Paper](https://arxiv.org/pdf/2302.14363.pdf)] [[Website](http://starydy.xyz/EINRUL/)] [[Code](https://github.com/StarRealMan/EINRUL)] [[Video](https://www.youtube.com/watch?v=wUp2I-X-IdI)]
* **NeRF-LOAM**: Neural Implicit Representation for Large-Scale Incremental LiDAR Odometry and Mapping, *ICCV, 2023*. [[Paper](https://arxiv.org/pdf/2303.10709.pdf)] [[Code](https://github.com/JunyuanDeng/NeRF-LOAM)]
* **NF-Atlas**: Multi-Volume Neural Feature Fields for Large Scale LiDAR Mapping, *RAL, 2023*. [[Paper](https://arxiv.org/pdf/2304.04624.pdf)] [[Website](https://yuxuan1206.github.io/NFAtlas/)] [[Code](https://github.com/yuxuan1206/NF-Atlas)]
* Accurate Implicit Neural Mapping with More Compact Representation in Large-scale Scenes Using Ranging Data, *RAL, 2023*. [[Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10238795)]
* **LONER**: LiDAR Only Neural Representations for Real-Time SLAM, *RAL, 2023*. [[Paper](https://arxiv.org/pdf/2309.04937.pdf)] [[Website](https://umautobots.github.io/loner)] [[Code](https://github.com/umautobots/LONER)]
* **PIN-SLAM**: LiDAR SLAM Using a Point-Based Implicit Neural Representation for Achieving Global Map Consistency, *TRO, 2024*. [[Paper](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/pan2024tro.pdf)] [[Code](https://github.com/PRBonn/PIN_SLAM)]
* Towards Large-Scale Incremental Dense Mapping using Robot-centric Implicit Neural Representation, *ICRA, 2024*.  [[Paper](https://arxiv.org/pdf/2306.10472.pdf)] [[Code](https://github.com/HITSZ-NRSL/RIM)] [[Video](https://www.youtube.com/watch?v=sHJ4lju6hsk)]
* **TNDF-Fusion**: Implicit Truncated Neural Distance Field for LiDAR Dense Mapping and Localization in Large Urban Environments, *RAL, 2024*.  [[Paper](https://ieeexplore.ieee.org/abstract/document/10598317)]

### Multimodal-SLAM
* Multi-Modal Neural Radiance Field for Monocular Dense SLAM with a Light-Weight ToF Sensor, *ICCV, 2023*. [[Paper](https://arxiv.org/pdf/2308.14383.pdf)] [[Website](https://zju3dv.github.io/tof_slam/)] [[Code](https://github.com/zju3dv/tof_slam)]
* NeuRSS: Enhancing AUV Localization and Bathymetric Mapping with Neural Rendering for Sidescan SLAM, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2405.05807)]
* **LIV-GaussMap**: LiDAR-Inertial-Visual Fusion for Real-time 3D Radiance Field Map Rendering, *RAL, 2024*. [[Paper](https://arxiv.org/pdf/2401.14857.pdf)] [[Code](https://github.com/sheng00125/LIV-GaussMap)]
* **HGS-Mapping**: Online Dense Mapping Using Hybrid Gaussian Representation in Urban Scenes, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.20159.pdf)]
* **MM3DGS SLAM**: Multi-modal 3D Gaussian Splatting for SLAM Using Vision, Depth, and Inertial Measurements, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2404.00923.pdf)] [[Website](https://vita-group.github.io/MM3DGS-SLAM/)]
* **MM-Gaussian**: 3D Gaussian-based Multi-modal Fusion for Localization and Reconstruction in Unbounded Scenes, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2404.04026.pdf)]
* **Gaussian-LIC**: Photo-realistic LiDAR-Inertial-Camera SLAM with 3D Gaussian Splatting, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2404.06926.pdf)]




## Planning & Navigation
* 3DGS-ReLoc: 3D Gaussian Splatting for Map Representation and Visual ReLocalization, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11367)] [[Website](https://arxiv.org/abs/2403.11367)]
* Beyond Uncertainty: Risk-Aware Active View Acquisition for Safe Robot Navigation and 3D Scene Understanding with FisherRF, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11396)] [[Website](https://arxiv.org/abs/2403.11396)]
* 3DGS-Calib: 3D Gaussian Splatting for Multimodal SpatioTemporal Calibration, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11577)] [[Website](https://arxiv.org/abs/2403.11577)]
* HO-Gaussian: Hybrid Optimization of 3D Gaussian Splatting for Urban Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20032.pdf)] [[Website](https://arxiv.org/abs/2403.20032)]
* SGD: Street View Synthesis with Gaussian Splatting and Diffusion Prior, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.20079.pdf)] [[Website](https://arxiv.org/abs/2403.20079)]
* **NeRFlow**: Neural Radiance Flow for 4D View Synthesis and Video Processing, *ICCV, 2021*. [[Paper](https://arxiv.org/abs/2012.09790)] [[Code](https://github.com/yilundu/nerflow)] [[Website](https://yilundu.github.io/nerflow/)] 
* **NeRF-Navigation**: Vision-Only Robot Navigation in a Neural Radiance World, *ICRA, 2022*. [[Paper](https://mikh3x4.github.io/nerf-navigation/assets/NeRF_Navigation.pdf)] [[Code](https://github.com/mikh3x4/nerf-navigation)] [[Website](https://mikh3x4.github.io/nerf-navigation/)] 
* Uncertainty Guided Policy for Active Robotic 3D Reconstruction using Neural Radiance Fields, *RAL, 2022*. [[Paper](https://arxiv.org/pdf/2209.08409.pdf)] [[Website](https://www.vis.xyz/pub/robotic-3d-scan-with-nerf/)] 
* **NeRF-dy**: 3D Neural Scene Representations for Visuomotor Control, *CoRL, 2021*. [[Paper](https://arxiv.org/abs/2107.04004)] [[Website](https://3d-representation-learning.github.io/nerf-dy/)] 
* **CompNeRFdyn**: Learning Multi-Object Dynamics with Compositional Neural Radiance Fields, *CoRL, 2022*. [[Paper](https://arxiv.org/pdf/2202.11855.pdf)] [[Website](https://dannydriess.github.io/compnerfdyn/)] 
* **PIFO**: Deep Visual Constraints: Neural Implicit Models for Manipulation Planning from Visual Input, *RAL, 2022*. [[Paper](https://arxiv.org/pdf/2112.04812.pdf)] [[Website](https://sites.google.com/view/deep-visual-constraints)] 
* **RedSDF**: Regularized Deep Signed Distance Fields for Reactive Motion Generation, *IROS, 2022*. [[Paper](https://arxiv.org/abs/2203.04739)] [[Website](https://irosalab.com/2022/02/28/redsdf/)] 
* **ESDF**: Sampling-free obstacle gradients and reactive planning in Neural Radiance Fields, *ICRA, 2022*. [[Paper](https://arxiv.org/abs/2205.01389)]
* Full-Body Visual Self-Modeling of Robot Morphologies, *Science Robotics, 2022*. [[Paper](https://arxiv.org/abs/2205.01389)] [[Code](https://github.com/BoyuanChen/visual-selfmodeling)] [[Website](https://robot-morphology.cs.columbia.edu/)]
* **CLIP-Fields**: Weakly Supervised Semantic Fields for Robotic Memory, *RSS, 2023*. [[Paper](https://arxiv.org/abs/2210.05663)] [[Code and Tutorials](https://github.com/notmahi/clip-fields)] [[Website](https://mahis.life/clip-fields/)]
* Renderable Neural Radiance Map for Visual Navigation, *CVPR, 2023*. [[Paper](https://arxiv.org/pdf/2303.00304.pdf)] [[Website](https://rllab-snu.github.io/projects/RNR-Map/)]
* **NeRF-VINS**: A Real-time Neural Radiance Field Map-based Visual-Inertial Navigation System, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2309.09295.pdf)]
* **Splat-Nav**: Safe Real-Time Robot Navigation in Gaussian Splatting Maps, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.02751.pdf)]
* **GaussNav**: Gaussian Splatting for Visual Navigation, *arXiv, 2024*. [[Paper](https://arxiv.org/pdf/2403.11625.pdf)] [[Code](https://github.com/XiaohanLei/GaussNav)] [[Website](https://xiaohanlei.github.io/projects/GaussNav/)]
* Active Implicit Reconstruction Using One-Shot View Planning, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2310.00685)]
* How Many Views Are Needed to Reconstruct an Unknown Object Using NeRF?, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2310.00684)]
* **GS-Planner**: A Gaussian-Splatting-based Planning Framework for Active High-Fidelity Reconstruction, *IROS, 2024*. [[Paper](https://arxiv.org/pdf/2405.10142)] [[Video](https://www.bilibili.com/video/BV1e1421S7Kh/)]
* NeRF-Enhanced Outpainting for Faithful Field-of-View Extrapolation, *ICRA, 2024*. [[Paper](https://arxiv.org/pdf/2309.13240)]
* Neural Visibility Field for Uncertainty-Driven Active Mapping, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2406.06948)] [[Website](https://sites.google.com/view/nvf-cvpr24/)] [[Code](https://github.com/GaTech-RL2/nvf_cvpr24)]


## Manipulation & RL
* **Ditto**: Building Digital Twins of Articulated Objects from Interaction, *CVPR, 2022*. [[Paper](https://arxiv.org/abs/2202.08227)] [[Code](https://github.com/UT-Austin-RPL/Ditto)] [[Website](https://ut-austin-rpl.github.io/Ditto/)]
* **Relational-NDF**:SE(3)-Equivariant Relational Rearrangement with Neural Descriptor Fields, *CoRL 2022*. [[Paper](https://arxiv.org/pdf/2211.09786.pdf)] [[Code](https://github.com/anthonysimeonov/relational_ndf)] [[Website](https://anthonysimeonov.github.io/r-ndf/)]
* **Neural Descriptor Fields**:SE(3)-Equivariant Object Representations for Manipulation, *ICRA, 2022*. [[Paper](https://arxiv.org/abs/2112.05124)] [[Code](https://github.com/anthonysimeonov/ndf_robot)] [[Website](https://yilundu.github.io/ndf/)]
* **Neural Motion Fields**: Encoding Grasp Trajectories as Implicit Value Functions, *RSS 2022*. [[Paper](https://arxiv.org/pdf/2206.14854.pdf)]  [[Video](https://youtu.be/B-pEhT1pi-Q)]
* **Grasping Field**: Learning Implicit Representations for Human Grasps, *3DV 2020*. [[Paper](https://arxiv.org/pdf/2008.04451.pdf)] [[Code](https://github.com/korrawe/grasping_field)] [[Video](https://youtu.be/J8x5i1FCgTQ)]
* **GIGA**: Synergies Between Affordance and Geometry: 6-DoF Grasp Detection via Implicit Representations, *RSS, 2021*. [[Paper](https://arxiv.org/abs/2104.01542)] [[Code](https://github.com/UT-Austin-RPL/GIGA)] [[Website](https://sites.google.com/view/rpl-giga2021)]
* **ObjectFolder**: A Dataset of Objects with Implicit Visual, Auditory, and Tactile Representations, *CoRL, 2021*. [[Paper](https://arxiv.org/pdf/2109.07991.pdf)] [[Code](https://github.com/rhgao/ObjectFolder)] [[Website](https://ai.stanford.edu/~rhgao/objectfolder/)]
* **ObjectFolder 2.0**: A Multisensory Object Dataset for Sim2Real Transfer, *CVPR, 2022*. [[Paper](https://arxiv.org/pdf/2204.02389.pdf)] [[Code](https://github.com/rhgao/ObjectFolder)] [[Website](https://ai.stanford.edu/~rhgao/objectfolder2.0/)]
* **Local Neural Descriptor Fields**: Locally Conditioned Object Representations for Manipulation, *ICRA, 2023*. [[Paper](https://arxiv.org/pdf/2302.03573.pdf)] [[Code](https://github.com/elchun/lndf_robot)] [[Website](https://elchun.github.io/lndf/)]
* **Equivariant Descriptor Fields**: SE(3)-Equivariant Energy-Based Models for End-to-End Visual Robotic Manipulation Learning, *ICLR, 2023*. [[Paper](https://openreview.net/forum?id=dnjZSPGmY5O)] [[Code](https://github.com/tomato1mule/edf)]
* Point'n Move: Interactive Scene Object Manipulation on Gaussian Splatting Radiance Fields, *arXiv*. [[Paper](https://arxiv.org/pdf/2311.16737.pdf)]

## Simulation & Human Interaction
* Control4D: Efficient 4D Portrait Editing with Text, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2305.20082.pdf)] [[Website](https://control4darxiv.github.io/)]
* Contrastive Gaussian Clustering: Weakly Supervised 3D Scene Segmentation, *arXiv*. [[Paper](https://arxiv.org/abs/2404.12784)]
* CoSSegGaussians: Compact and Swift Scene Segmenting 3D Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.05925.pdf)] [[Website](https://david-dou.github.io/CoSSegGaussians/)] [[Code](https://DavidDou.github.io/CoSSegGaussians)]
* TIP-Editor: An Accurate 3D Editor Following Both Text-Prompts And Image-Prompts, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.14828.pdf)] [[Website](https://zjy526223908.github.io/TIP-Editor/)]
* Segment Anything in 3D Gaussians, *arXiv*. [[Paper](https://browse.arxiv.org/pdf/2401.17857.pdf)]
* GSEdit: Efficient Text-Guided Editing of 3D Objects via Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.05154.pdf)]
* GaussCtrl: Multi-View Consistent Text-Driven 3D Gaussian Splatting Editing, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.08733.pdf)]
* View-Consistent 3D Editing with Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11868.pdf)]
* Gaussian Frosting: Editable Complex Radiance Fields with Real-Time Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.14554)] [[Website](https://anttwo.github.io/frosting/)] [[Code](https://github.com/Anttwo/Frosting)]
* ICE-G: Image Conditional Editing of 3D Gaussian Splats, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2406.08488)] [[Website](https://ice-gaussian.github.io/)]
* GaussianEditor: Swift and Controllable 3D Editing with Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.14521.pdf)] [[Website](https://buaacyw.github.io/gaussian-editor/)] [[Code](https://github.com/buaacyw/GaussianEditor)]
* GaussianEditor: Editing 3D Gaussians Delicately with Text Instructions, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2311.16037.pdf)] [[Website](https://gaussianeditor.github.io/)]
* Gaussian Grouping: Segment and Edit Anything in 3D Scenes, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2312.00732.pdf)] [[Code](https://github.com/lkeab/gaussian-grouping)]
* 

## MISC
### 14. SyncTweedies: A General Generative Framework Based on Synchronized Diffusions   
**Authors**: Jaihoon Kim, Juil Koo, Kyeongmin Yeo, Minhyuk Sung  

<details span>
<summary><b>Abstract</b></summary>
We introduce a general framework for generating diverse visual content, including ambiguous images, panorama images, mesh textures, and Gaussian splat textures, by synchronizing multiple diffusion processes. We present exhaustive investigation into all possible scenarios for synchronizing multiple diffusion processes through a canonical space and analyze their characteristics across applications. In doing so, we reveal a previously unexplored case: averaging the outputs of Tweedie's formula while conducting denoising in multiple instance spaces. This case also provides the best quality with the widest applicability to downstream tasks. We name this case SyncTweedies. In our experiments generating visual content aforementioned, we demonstrate the superior quality of generation by SyncTweedies compared to other synchronization methods, optimization-based and iterative-update-based methods.
</details>

[📄 Paper](https://arxiv.org/pdf/2403.14370) | [🌐 Project Page](https://synctweedies.github.io/)
### 10. EgoLifter: Open-world 3D Segmentation for Egocentric Perception 
**Authors**: Qiao Gu, Zhaoyang Lv, Duncan Frost, Simon Green, Julian Straub, Chris Sweeney 

<details span>
<summary><b>Abstract</b></summary>
In this paper we present EgoLifter, a novel system that can automatically segment scenes captured from egocentric sensors into a complete decomposition of individual 3D objects. The system is specifically designed for egocentric data where scenes contain hundreds of objects captured from natural (non-scanning) motion. EgoLifter adopts 3D Gaussians as the underlying representation of 3D scenes and objects and uses segmentation masks from the Segment Anything Model (SAM) as weak supervision to learn flexible and promptable definitions of object instances free of any specific object taxonomy. To handle the challenge of dynamic objects in ego-centric videos, we design a transient prediction module that learns to filter out dynamic objects in the 3D reconstruction. The result is a fully automatic pipeline that is able to reconstruct 3D object instances as collections of 3D Gaussians that collectively compose the entire scene. We created a new benchmark on the Aria Digital Twin dataset that quantitatively demonstrates its state-of-the-art performance in open-world 3D segmentation from natural egocentric input. We run EgoLifter on various egocentric activity datasets which shows the promise of the method for 3D egocentric perception at scale. 
</details>

  [📄 Paper](https://arxiv.org/pdf/2403.18118.pdf) | [🌐 Project Page](https://egolifter.github.io/) | [💻 Code (not yet)]() 
  
### 11. InFusion: Inpainting 3D Gaussians via Learning Depth Completion from Diffusion Prior 
**Authors**: Zhiheng Liu, Hao Ouyang, Qiuyu Wang, Ka Leong Cheng, Jie Xiao, Kai Zhu, Nan Xue, Yu Liu, Yujun Shen, Yang Cao

<details span>
<summary><b>Abstract</b></summary>
3D Gaussians have recently emerged as an efficient representation for novel view synthesis. This work studies its editability with a particular focus on the inpainting task, which aims to supplement an incomplete set of 3D Gaussians with additional points for visually harmonious rendering. Compared to 2D inpainting, the crux of inpainting 3D Gaussians is to figure out the rendering-relevant properties of the introduced points, whose optimization largely benefits from their initial 3D positions. To this end, we propose to guide the point initialization with an image-conditioned depth completion model, which learns to directly restore the depth map based on the observed image. Such a design allows our model to fill in depth values at an aligned scale with the original depth, and also to harness strong generalizability from largescale diffusion prior. Thanks to the more accurate depth completion, our approach, dubbed InFusion, surpasses existing alternatives with sufficiently better fidelity and efficiency under various complex scenarios. We further demonstrate the effectiveness of InFusion with several practical applications, such as inpainting with user-specific texture or with novel object insertion.
</details>

  [📄 Paper](https://arxiv.org/pdf/2404.11613) | [🌐 Project Page](https://johanan528.github.io/Infusion/) | [💻 Code](https://github.com/ali-vilab/infusion) 

### 12. Gaga: Group Any Gaussians via 3D-aware Memory Bank
**Authors**: Weijie Lyu, Xueting Li, Abhijit Kundu, Yi-Hsuan Tsai, Ming-Hsuan Yang

<details span>
<summary><b>Abstract</b></summary>
We introduce Gaga, a framework that reconstructs and segments open-world 3D scenes by leveraging inconsistent 2D masks predicted by zero-shot segmentation models. Contrasted to prior 3D scene segmentation approaches that heavily rely on video object tracking, Gaga utilizes spatial information and effectively associates object masks across diverse camera poses. By eliminating the assumption of continuous view changes in training images, Gaga demonstrates robustness to variations in camera poses, particularly beneficial for sparsely sampled images, ensuring precise mask label consistency. Furthermore, Gaga accommodates 2D segmentation masks from diverse sources and demonstrates robust performance with different open-world zero-shot segmentation models, significantly enhancing its versatility. Extensive qualitative and quantitative evaluations demonstrate that Gaga performs favorably against state-of-the-art methods, emphasizing its potential for real-world applications such as scene understanding and manipulation.
</details>

  [📄 Paper](https://arxiv.org/pdf/2404.07977.pdf) | [🌐 Project Page](https://www.gaga.gallery/) | [💻 Code](https://github.com/weijielyu/Gaga)

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

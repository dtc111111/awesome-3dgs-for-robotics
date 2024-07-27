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

## 3DGS Foundation Model
* 3D Gaussian Splatting for Real-Time Radiance Field Rendering, **SIGGRAPH, 2023**. [[Paper](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/3d_gaussian_splatting_low.pdf)] [[Website](https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/)]
* 2D Gaussian Splatting for Geometrically Accurate Radiance Fields, **SIGGRAPH, 2024**. [[Paper](https://arxiv.org/pdf/2403.17888)] [[Website](https://surfsplatting.github.io/)]  [[Code](https://github.com/hbb1/2d-gaussian-splatting)]
* Mip-splatting: Alias-free 3d gaussian splatting, **CVPR, 2024**. [[Paper](https://openaccess.thecvf.com/content/CVPR2024/papers/Yu_Mip-Splatting_Alias-free_3D_Gaussian_Splatting_CVPR_2024_paper.pdf)] [[Website](https://niujinshuchong.github.io/mip-splatting/)]  [[Code](https://github.com/autonomousvision/mip-splatting)]
* End-to-End Rate-Distortion Optimized 3D Gaussian Representation, **ECCV, 2024**. [[Paper](https://arxiv.org/pdf/2406.01597.pdf)] [[Website](https://arxiv.org/abs/2406.01597)] [[Code](https://github.com/USTC-IMCL/RDO-Gaussian)]

## Perception
### Multi-Modal
* GaussianBody: Clothed Human Reconstruction via 3d Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.09720.pdf)] [[Website](https://arxiv.org/abs/2401.09720)]
* PSAvatar: A Point-based Morphable Shape Model for Real-Time Head Avatar Creation with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2401.12900.pdf)] [[Website](https://arxiv.org/abs/2401.12900)]
* Rig3DGS: Creating Controllable Portraits from Casual Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.03723.pdf)] [[Website](http://shahrukhathar.github.io/2024/02/05/Rig3DGS.html)]
* HeadStudio: Text to Animatable Head Avatars with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.06149.pdf)] [[Website](https://zhenglinzhou.github.io/HeadStudio-ProjectPage/)] [[Code](https://github.com/ZhenglinZhou/HeadStudio/)]
* ImplicitDeepfake: Plausible Face-Swapping through Implicit Deepfake Generation using NeRF and Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.06390.pdf)] [[Website](https://arxiv.org/abs/2402.06390)] [[Code](https://github.com/quereste/implicit-deepfake)]
* GaussianHair: Hair Modeling and Rendering with Light-aware Gaussians, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.10483)] [[Website](https://arxiv.org/abs/2402.10483)]
* GVA: Reconstructing Vivid 3D Gaussian Avatars from Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.16607.pdf)] [[Website](https://3d-aigc.github.io/GEA/)]
* SplattingAvatar: Realistic Real-Time Human Avatars with Mesh-Embedded Gaussian Splatting, **CVPR, 2024**. [[Paper](https://arxiv.org/pdf/2403.05087.pdf)]  [[Website](https://initialneil.github.io/SplattingAvatar)] [[Code](https://github.com/initialneil/SplattingAvatar)]
* SplatFace: Gaussian Splat Face Reconstruction Leveraging an Optimizable Surface, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.18784)] [[Website](https://arxiv.org/abs/2403.18784)]
* HAHA: Highly Articulated Gaussian Human Avatars with Textured Mesh Prior, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.01053)] [[Website](https://arxiv.org/abs/2404.01053)]
* Gaussian Splatting Decoder for 3D‑aware Generative Adversarial Networks, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2404.10625)]  [[Website](https://florian-barthel.github.io/gaussian_decoder/index.html)] [[Code](https://github.com/fraunhoferhhi/gaussian_gan_decoder)]
* GoMAvatar: Efficient Animatable Human Modeling from Monocular Video Using Gaussians-on-Mesh, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.07991)]  [[Website](https://wenj.github.io/GoMAvatar/)] [[Code](https://github.com/wenj/GoMAvatar)]
* OccGaussian: 3D Gaussian Splatting for Occluded Human Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.07991)]  [[Website](https://arxiv.org/abs/2404.07991)]
* Guess The Unseen: Dynamic 3D Scene Reconstruction from Partial 2D Glimpses, **CVPR, 2024**. [[Paper](https://arxiv.org/abs/2404.14410)]  [[Website](https://snuvclab.github.io/gtu/)] [[Code](https://github.com/snuvclab/gtu/)]

## Mapping & Localization
### 3D Reconstruction


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
* 4D Gaussian Splatting: Towards Efficient Novel View Synthesis for Dynamic Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2402.03307)] [[Website](https://arxiv.org/abs/2402.03307)]
* GaussianFlow: Splatting Gaussian Dynamics for 4D Content Creation, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.12365)] [[Website](https://zerg-overmind.github.io/GaussianFlow.github.io/)] [[Code](https://github.com/Zerg-Overmind/GaussianFlow)]
* Motion-aware 3D Gaussian Splatting for Efficient Dynamic Scene Reconstruction, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11447)] [[Website](https://arxiv.org/abs/2403.11447)]
* Bridging 3D Gaussian and Mesh for Freeview Video Rendering, *arXiv*. [[Paper](https://arxiv.org/pdf/2403.11453)] [[Website](https://arxiv.org/abs/2403.11453)]
* Per-Gaussian Embedding-Based Deformation for Deformable 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.03613)] [[Website](https://jeongminb.github.io/e-d3dgs/)] [[Code](https://github.com/JeongminB/E-D3DGS)]
* DreamScene4D: Dynamic Multi-Object Scene Generation from Monocular Videos, *arXiv*. [[Paper](https://arxiv.org/pdf/2405.02280)] [[Website](https://dreamscene4d.github.io/)] [[Code](https://github.com/dreamscene4d/dreamscene4d)]
* 3D Geometry-aware Deformable Gaussian Splatting for Dynamic View Synthesis, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2404.06270)] [[Website](https://npucvr.github.io/GaGS/)]
* Dynamic 3D Gaussians: Tracking by Persistent Dynamic View Synthesis, *3DV, 2024*. [[Paper](https://dynamic3dgaussians.github.io/paper.pdf)] [[Website](https://dynamic3dgaussians.github.io/)] [[Code](https://github.com/JonathonLuiten/Dynamic3DGaussians)]
* Deformable 3D Gaussians for High-Fidelity Monocular Dynamic Scene Reconstruction, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2309.13101.pdf)] [[Website](https://ingra14m.github.io/Deformable-Gaussians/)] [[Code](https://github.com/ingra14m/Deformable-3D-Gaussians)]
* 4D Gaussian Splatting for Real-Time Dynamic Scene Rendering, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2310.08528.pdf)] [[Website](https://guanjunwu.github.io/4dgs/)] [[Code](https://github.com/hustvl/4DGaussians)]
* Real-time Photorealistic Dynamic Scene Representation and Rendering with 4D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2310.10642.pdf)] [[Website](https://github.com/fudan-zvg/4d-gaussian-splatting)]
* A Compact Dynamic 3D Gaussian Representation for Real-Time Dynamic View Synthesis, *ECCV, 2024*. [[Paper](https://arxiv.org/pdf/2311.12897.pdf)] [[Website](https://compactdynamic3dgaussian.github.io/)] [[Code](https://github.com/raven38/EfficientDynamic3DGaussian)]
* DynMF: Neural Motion Factorization for Real-time Dynamic View Synthesis with 3D Gaussian Splatting, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.00112.pdf)] [[Website](https://agelosk.github.io/dynmf/)] [[Code](https://github.com/agelosk/dynmf)]
* SC-GS: Sparse-Controlled Gaussian Splatting for Editable Dynamic Scenes, *CVPR, 2024*. [[Paper](https://yihua7.github.io/SC-GS-web/materials/SC_GS_Arxiv.pdf)] [[Website](https://yihua7.github.io/SC-GS-web/)] [[Code](https://github.com/yihua7/SC-GS)]
* Gaussian-Flow: 4D Reconstruction with Dynamic 3D Gaussian Particle, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2310.08528.pdf)] [[Website](https://nju-3dv.github.io/projects/Gaussian-Flow)]
* GauFRe: Gaussian Deformation Fields for Real-time Dynamic Novel View Synthesis, *arXiv*. [[Paper](https://arxiv.org/pdf/2312.11458.pdf)] [[Website](https://lynl7130.github.io/gaufre/index.html)]
* Spacetime Gaussian Feature Splatting for Real-Time Dynamic View Synthesis, *CVPR, 2024*. [[Paper](https://arxiv.org/pdf/2312.16812.pdf)] [[Website](https://oppo-us-research.github.io/SpacetimeGaussians-website/)] [[Code](https://github.com/oppo-us-research/SpacetimeGaussians)]
* SWinGS: Sliding Windows for Dynamic 3D Gaussian Splatting, *ECCV, 2024*. [[Paper](https://arxiv.org/pdf/2312.13308.pdf)] [[Website](https://arxiv.org/abs/2312.13308)] [[Code](https://github.com/tyhuang0428/DreamPhysics)]

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
* PIN-SLAM: LiDAR SLAM Using a Point-Based Implicit Neural Representation for Achieving Global Map Consistency, *TRO, 2024*. [[Paper](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/pan2024tro.pdf)] [[Code](https://github.com/PRBonn/PIN_SLAM)]
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
* TCLC-GS: Tightly Coupled LiDAR-Camera Gaussian Splatting for Surrounding Autonomous Driving Scenes, *arXiv*. [[Paper](https://arxiv.org/pdf/2404.02410.pdf)] [[Website](https://arxiv.org/abs/2404.02410)]
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
* Reinforcement Learning with Neural Radiance Fields, *NeurIPS, 2022*. [[Paper](https://dannydriess.github.io/papers/22-driess-NeRF-RL.pdf)]  [[Website](https://dannydriess.github.io/nerf-rl/)]
* **Neural Motion Fields**: Encoding Grasp Trajectories as Implicit Value Functions, *RSS 2022*. [[Paper](https://arxiv.org/pdf/2206.14854.pdf)]  [[Video](https://youtu.be/B-pEhT1pi-Q)]
* **Grasping Field**: Learning Implicit Representations for Human Grasps, *3DV 2020*. [[Paper](https://arxiv.org/pdf/2008.04451.pdf)] [[Code](https://github.com/korrawe/grasping_field)] [[Video](https://youtu.be/J8x5i1FCgTQ)]
* **Dex-NeRF**: Using a Neural Radiance Field to Grasp Transparent Objects, *CoRL, 2021*. [[Paper](https://arxiv.org/abs/2110.14217)]  [[Website](https://sites.google.com/view/dex-nerf)]
* **NeRF-Supervision**: Learning Dense Object Descriptors from Neural Radiance Fields, *ICRA, 2022*. [[Paper](https://arxiv.org/abs/2203.01913)] [[Code](https://github.com/yenchenlin/nerf-supervision-public)] [[Website](https://yenchenlin.me/nerf-supervision/)]
* **GIGA**: Synergies Between Affordance and Geometry: 6-DoF Grasp Detection via Implicit Representations, *RSS, 2021*. [[Paper](https://arxiv.org/abs/2104.01542)] [[Code](https://github.com/UT-Austin-RPL/GIGA)] [[Website](https://sites.google.com/view/rpl-giga2021)]
* **NeuralGrasps**: Learning Implicit Representations for Grasps of Multiple Robotic Hands, *CoRL, 2022*. [[Paper](https://arxiv.org/abs/2207.02959)] [[Website](https://irvlutd.github.io/NeuralGrasps/)]
* **ObjectFolder**: A Dataset of Objects with Implicit Visual, Auditory, and Tactile Representations, *CoRL, 2021*. [[Paper](https://arxiv.org/pdf/2109.07991.pdf)] [[Code](https://github.com/rhgao/ObjectFolder)] [[Website](https://ai.stanford.edu/~rhgao/objectfolder/)]
* **ObjectFolder 2.0**: A Multisensory Object Dataset for Sim2Real Transfer, *CVPR, 2022*. [[Paper](https://arxiv.org/pdf/2204.02389.pdf)] [[Code](https://github.com/rhgao/ObjectFolder)] [[Website](https://ai.stanford.edu/~rhgao/objectfolder2.0/)]
* **NeRF2Real**: Sim2real Transfer of Vision-guided Bipedal Motion Skills using Neural Radiance Fields, *ICRA, 2023*. [[Paper](https://arxiv.org/pdf/2210.04932.pdf)] [[Website](https://sites.google.com/view/nerf2real/home)]
* Neural Fields for Robotic Object Manipulation from a Single Image / One-shot neural fields for 3d object understanding *arXiv, 2022*. [[Paper](https://arxiv.org/pdf/2210.12126.pdf)] [[Website](https://nerfgrasp.github.io/)]
* **Local Neural Descriptor Fields**: Locally Conditioned Object Representations for Manipulation, *ICRA, 2023*. [[Paper](https://arxiv.org/pdf/2302.03573.pdf)] [[Code](https://github.com/elchun/lndf_robot)] [[Website](https://elchun.github.io/lndf/)]
* **Equivariant Descriptor Fields**: SE(3)-Equivariant Energy-Based Models for End-to-End Visual Robotic Manipulation Learning, *ICLR, 2023*. [[Paper](https://openreview.net/forum?id=dnjZSPGmY5O)] [[Code](https://github.com/tomato1mule/edf)]
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

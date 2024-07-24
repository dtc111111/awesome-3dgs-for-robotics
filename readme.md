# Awesome 3D Gaussian Splatting for Robotics [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

This repo contains a curative list of **3D Gaussian Splatting papers relating to the Robotics domain**.

#### Please feel free to send me [pull requests](https://github.com/dtc111111/awesome-3dgs-for-robotics) or [email](mailto:dengtianchen@sjtu.edu.cn) to add papers! <br>

If you find this repository useful, please consider [citing](#citation) and STARing this list. Feel free to share this list with others!

For an overview of **3D Gaussian Splatting**, checkout the Survey ([Neural Volume Rendering: NeRF And Beyond](https://arxiv.org/abs/2101.05204) and [NeRF: Neural Radiance Field in 3D Vision, A Comprehensive Review](https://arxiv.org/pdf/2210.00379.pdf)), Blog post ([NeRF Explosion 2020](https://dellaert.github.io/NeRF/)) and Collection ([awesome-NeRF](https://github.com/yenchenlin/awesome-NeRF))

---

## Overview

  - [NeRF Foundation Model](#nerf-general-model)

  - [SLAM](#slam)
    - [Visual-SLAM](#Visual-SLAM)
    - [Lidar-SLAM](#Lidar-SLAM)
    - [Multimodal-SLAM](#Multimodal-SLAM)

  - [Robotics](#Robotics)

    - [Manipulation/RL](#manipulationrl)

    - [Planning/Navigation](#planningnavigation)

    - [Localization](#localization)

  - [Citation](#citation)

---
## 3D Gaussian Splatting Survey

#### [S0] A Survey on 3D Gaussian Splatting
- **🧑‍🔬 作者**：Guikun Chen, Wenguan Wang
- **🏫 单位**：Zhejiang University
- **🔗 链接**：[[中英摘要](./abs/2401.03890.md)] [[arXiv:2401.03890](https://arxiv.org/abs/2401.03890)]
- **📝 说明**：🔥 首篇综述

#### [S1] 3D Gaussian as a New Vision Era: A Survey
- **🧑‍🔬 作者**：Ben Fei, Jingyi Xu, Rui Zhang, Qingyuan Zhou, Weidong Yang, Ying He
- **🏫 单位**：Fudan University ⟐ Nanyang Technological University
- **🔗 链接**：[[中英摘要](./abs/2402.07181.md)] [[arXiv:2402.07181](https://arxiv.org/abs/2402.07181)]
- **📝 说明**：🏆 Accepted to IEEE TVCG 2024

#### [S2] Recent Advances in 3D Gaussian Splatting
- **🧑‍🔬 作者**：Tong Wu, Yu-Jie Yuan, Ling-Xiao Zhang, Jie Yang, Yan-Pei Cao, Ling-Qi Yan, Lin Gao
- **🏫 单位**：Chinese Academy of Sciences ⟐ VAST ⟐  University of California
- **🔗 链接**：[[中英摘要](./abs/2403.11134.md)] [[arXiv:2403.11134](https://arxiv.org/abs/2403.11134)]
- **📝 说明**：🔥 第三篇综述，涵盖了更多最新进展

#### [S3] Gaussian Splatting: 3D Reconstruction and Novel View Synthesis, a Review
- **🧑‍🔬 作者**：Anurag Dalal, Daniel Hagen, Kjell G. Robbersmyr, Kristian Muri Knausgård
- **🏫 单位**：University of Agder
- **🔗 链接**：[[中英摘要](./abs/2405.03417.md)] [[arXiv:2405.03417](https://arxiv.org/abs/2405.03417)]
- **📝 说明**：🔥 第四篇综述

#### [S4] 3DGS.zip: A survey on 3D Gaussian Splatting Compression Methods
- **🧑‍🔬 作者**：Milena T. Bagdasarian, Paul Knoll, Florian Barthel, Anna Hilsmann, Peter Eisert, Wieland Morgenstern
- **🏫 单位**：Fraunhofer Heinrich Hertz ⟐ Humboldt University of Berlin
- **🔗 链接**：[[中英摘要](./abs/2407.09510.md)] [[arXiv:2407.09510](https://arxiv.org/abs/2407.09510)]
- **📝 说明**：🧩 高斯压缩综述

---

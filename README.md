# Jinyuan Yu

CEO, 深圳市视元引擎有限公司.

**Seeking research and industry collaborators in 3D vision, neural rendering, computer graphics, and avatar reconstruction.**

I lead 深圳市视元引擎有限公司, developing low-cost 2D-to-3D conversion, 3D content generation, and hardware-interoperable glasses-free 3D display systems.

[Email](mailto:522066928@qq.com) | [Public CV](Jinyuan_Yu_CV_Public.pdf) | [GitHub](https://github.com/jinyuanyu)

<!-- Add verified Google Scholar, ORCID, and personal website URLs here when available. -->

## Research Focus

My research focuses on **3D/4D computer vision and geometry-aware generative modeling**, with particular interests in depth estimation, novel-view synthesis, 3D Gaussian Splatting, human avatars, and evidence-preserving medical visualization.

I work across data preparation, geometry, PyTorch training, evaluation, GPU inference, and interactive visualization, with a focus on reliable monocular and sparse-view reconstruction under occlusion and limited observations.

## Selected Research

### [MALA: Temporal-Spatial Remote-Sensing Reconstruction](https://github.com/jinyuanyu/MALA)

**Research question.** How can missing satellite observations be reconstructed from temporal evidence without smoothing away genuine spatial change?

**My contribution.** I developed the EMAE temporal masked-autoencoder baseline and the MALA extension, combining temporal attention, multi-scale spatial features, explicit masks, and optional LaMA initialization.

**Main result.** Across four currently reported representative cases, MALA averages **31.05 dB PSNR**, compared with **28.89 dB** for EMAE. The related paper is under review, and the work produced two patent applications.

### [DepthWarpVS: Real-Time Novel-View Synthesis](https://github.com/jinyuanyu/depth_warp_vs)

**Research question.** Can explicit depth reprojection and localized completion synthesize stable multi-view output more efficiently than regenerating every target view?

**My contribution.** I designed the depth-warping system, the `hole`/`valid`/`pollute` reliability representation, the lightweight MGMI completion network, and the synthetic defect-generation pipeline.

**Main result.** The research prototype reports approximately **5 ms per 4K target-view completion** and approximately **15 FPS for 11-view output on one RTX 4090**. Related work was accepted at ICDT 2026.

### [VDA Absolute Depth Distillation](https://github.com/jinyuanyu/VDA-Absolute-Depth-Distillation)

**Research question.** Can frozen relative-depth features predict per-frame scale and shift parameters for scene-conditioned metric-depth calibration?

**My contribution.** I adapted Video Depth Anything for single-image feature extraction, designed reciprocal-affine calibration, generated Depth Pro pseudo-labels, and trained a lightweight scale head while freezing the backbone.

**Main result.** The current 1,800-frame scene snapshot reports teacher-referenced MSE of **0.1294/0.2248** on two held-out cameras. These values measure in-scene teacher agreement, not cross-scene generalization.

### [FlashAvatar-DepthFusion](https://github.com/jinyuanyu/FlashAvatar-DepthFusion)

**Research question.** Can relative monocular depth regularize underconstrained side-view facial geometry in RGB-only avatar reconstruction?

**My contribution.** I extended FlashAvatar with aligned depth loading, scale-invariant Pearson-correlation supervision, conservative face masks, preprocessing validation, and novel-view comparison tools.

**Main result.** The depth-supervision branch runs end to end and has produced qualitative cross-view comparisons on three identities. A controlled quantitative benchmark is not yet available.

### [Knee MRI 3D Communication](https://github.com/jinyuanyu/knee-mri-3d-communication)

**Research question.** How can MRI evidence, reviewed semantic structures, and local appearance representations be combined without making clinically unsupported claims?

**My contribution.** I built the privacy-minimized data schema and export tools, WebGL2 volume/cutaway viewer, segmentation interfaces, MRI-derived Gaussian pipeline, hybrid manifest, and automated tests.

**Main result.** The public prototype delivers one authorized privacy-minimized case with four MRI sequences and a 47,443-Gaussian representation. It is an engineering prototype, not a clinically validated system.

## Publications and Research Outputs

- **DWvs: Depth-Guided Image Warping and Hole Filling for Novel View Synthesis.** Co-author, ICDT 2026, accepted.
- **Research on Spectral Interpolation and Extrapolation of Remote Sensing Images Based on Temporal Generation Model.** Under review.
- Patent application CN202511188342.5: temporal-stability partitioning and Transformer-LaMA remote-sensing interpolation.
- Patent application 202511314521.9: masked-autoencoding interpolation for sea-surface reflectance products.
- Patent application CN202311554601.2: multi-vehicle urban sensing optimization.

## Background

- **CEO**, 深圳市视元引擎有限公司, Present.
- **Research Assistant**, Department of Electrical and Electronic Engineering, Southern University of Science and Technology, 2025-2026.
- **M.S. in Computer Technology**, Shenzhen Institute of Advanced Technology, Chinese Academy of Sciences, 2025.
- **B.S. in Computer Science and Technology**, Shandong University of Science and Technology, 2019.

## Technical Areas

`3D Gaussian Splatting` `Neural Rendering` `Novel-View Synthesis` `Monocular Depth` `PyTorch` `CUDA/GPU Systems` `Temporal Modeling` `Optimization`

For research or industry collaboration inquiries, contact [522066928@qq.com](mailto:522066928@qq.com).

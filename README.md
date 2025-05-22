Official repository of our CVPR 2025 paper ”Detection-Friendly Nonuniformity Correction: A Union Framework for Infrared UAV Target Detection“ [![arXiv](https://img.shields.io/badge/arXiv-2504.04012-b31b1b.svg)](https://arxiv.org/abs/2504.04012)

## Detection-Friendly Nonuniformity Correction: A Union Framework for Infrared UAV Target Detection [[PDF](https://arxiv.org/abs/2504.04012)]


Authors: Houzhang Fang<sup>1</sup>, Xiaolin Wang<sup>1</sup>, Zengyang Li<sup>1</sup>, Lu Wang<sup>1</sup>, Qingshan Li<sup>1</sup>, Yi Chang<sup>2</sup>, Luxin Yan<sup>2</sup>
  
<sup>1</sup>Xidian University,  <sup>2</sup>Huazhong University of Science and Technology

## News: Our work has been selected as a *highlight*  at the CVPR 2025 conference!

## Abstract

Infrared unmanned aerial vehicle (UAV) images captured using thermal detectors are often affected by temperature-dependent low-frequency nonuniformity, which significantly reduces the contrast of the images. Detecting UAV targets under nonuniform conditions is crucial in UAV surveillance applications. Existing methods typically treat infrared nonuniformity correction (NUC) as a preprocessing step for detection, which leads to suboptimal performance. Balancing the two tasks while enhancing detection-beneficial information remains challenging. In this paper, we present a detection-friendly union framework, termed UniCD, that simultaneously addresses both infrared NUC and UAV target detection tasks in an end-to-end manner. We first model NUC as a small number of parameter estimation problem jointly driven by priors and data to generate detection-conducive images. Then, we incorporate a new auxiliary loss with target mask supervision into the backbone of the infrared UAV target detection network to strengthen target features while suppressing the background. To better balance correction and detection, we introduce a detection-guided self-supervised loss to reduce feature discrepancies between the two tasks, thereby enhancing detection robustness to varying nonuniformity levels. Additionally, we construct a new benchmark composed of 50,000 infrared images in various nonuniformity types, multi-scale UAV targets and rich backgrounds with target annotations, called IRBFD. Extensive experiments on IRBFD demonstrate that our UniCD is a robust union framework for NUC and UAV target detection while achieving real-time processing capabilities.



## Dataset Download Link

The dataset used in our paper can be downloaded via the following link:

- Download Dataset Here -[Baidu Netdisk](<https://pan.baidu.com/s/1cgzAo8ZLIqplCV5tCIOldw?pwd=ujdm >) ,  [Google Drive(TODO)](<>)

## NUC Software

We have developed an correction software, allowing users to upload various non-uniform images for real-time processing. Our method does not require retraining and demonstrates excellent universal applicability across diverse scenarios.
Our correction software currently only provides processing results based on the non-uniformity correction algorithm from the CVPR paper and can run on both Linux and Windows systems.

Usage steps:

- **Step 1.** Click the “Select Images” button to load images (multiple images can be loaded). You can also select an entire image folder for batch processing.
- **Step 2.** Choose the output folder where the processed results will be saved. If this step is skipped, the results will be saved by default in the folder where the images were selected in step 1.
- **Step 3.** Click the “Process Images” button. The software will save both the corrected images and the estimated bias field images.

 Download software Here -[Google Drive](<https://drive.google.com/file/d/1UrBzFC6swyTVb_8g7ovrpEm3LDVXC8km/view?usp=drive_link>)

Key Features:

- **No Retraining Required**: Immediately applicable to a wide range of infrared nonuniformity images.
- **Universal Applicability**: Outstanding performance across different  scenes.
- **Real-time Processing**: Supports real-time online demonstration for quick validation.

## Citation
If you find our work useful for your research, please consider citing our paper:
```
@inproceedings{2025CVPR_UniCD,
    title     = {Detection-Friendly Nonuniformity Correction: A Union Framework for Infrared {UAV} Target Detection},
    author    = {Houzhang Fang; Xiaolin Wang; Zengyang Li; Lu Wang; Qingshan Li; Yi Chang; Luxin Yan},
    booktitle = {IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    year      = {2025},
    pages     = { },
}
```

In additoin to the above paper, please also consider citing the following references. Thank you!
```
@article{2024TGRS_SCINet,
  title     = {{SCINet}: Spatial and Contrast Interactive Super-Resolution Assisted Infrared {UAV} Target Detection},
  author    = {Houzhang Fang; Lan Ding; Xiaolin Wang; Yi Chang; Luxin Yan; Li Liu; Jinrui Fang},
  journal   = {IEEE Transactions on Geoscience and Remote Sensing},
  volume    = {62},
  year      = {2024},
  pages     = {1-22},
}
@ARTICLE{2023TII_DAGNet,
  title     =  {Differentiated Attention Guided Network Over Hierarchical and Aggregated Features for Intelligent {UAV} Surveillance},
  author    =  {Houzhang Fang and Zikai Liao and Xuhua Wang and Yi Chang and Luxin Yan},
  journal   =  {IEEE Transactions on Industrial Informatics}, 
  year      =  {2023},
  volume    =  {19},
  number    =  {9},
  pages     =  {9909-9920},
  }
@inproceedings{2023ACMMM_DANet,
title       =  {{DANet}: Multi-scale {UAV} Target Detection with Dynamic Feature Perception and Scale-aware Knowledge Distillation},
author      =  {Houzhang Fang and Zikai Liao and Lu Wang and Qingshan Li and Yi Chang and Luxin Yan and Xuhua Wang},
booktitle   =  {Proceedings of the 31st ACM International Conference on Multimedia (ACMMM)},
pages       =  {2121-2130},
year        =  {2023},
}
@ARTICLE{2022TIMFang,
  title     =  {Infrared Small {UAV} Target Detection Based on Depthwise Separable Residual Dense Network and Multiscale Feature Fusion},
  author    =  {Houzhang Fang and Lan Ding and Liming Wang and Yi Chang and Luxin Yan and Jinhui Han},
  journal   =  {IEEE Transactions on Instrumentation and Measurement}, 
  year      =  {2022},
  volume    =  {71},
  number    =  {},
  pages     =  {1-20},
}
```





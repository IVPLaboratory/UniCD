# UniCD
Official repositoryof our CVPR 2025 paper ”Detection-Friendly Nonuniformity Correction: A Union Framework for Infrared UAV Target Detection“


# Detection-Friendly Nonuniformity Correction: A Union Framework for Infrared UAV Target Detection


Houzhang Fang<sup>1</sup>, Xiaolin Wang<sup>1</sup>, Zengyang Li<sup>1</sup>, Lu Wang<sup>1</sup>, Qingshan Li<sup>1</sup>, Yi Chang<sup>2</sup>, Luxin Yan<sup>2</sup>
  
<sup>1</sup>Xidian University,  <sup>2</sup>Huazhong University of Science and Technology

## Abstract

Infrared unmanned aerial vehicle (UAV) images captured using thermal detectors are often affected by temperature-dependent low-frequency nonuniformity, which significantly reduces the contrast of the images. Detecting UAV targets under nonuniform conditions is crucial in UAV surveillance applications. Existing methods typically treat infrared nonuniformity correction (NUC) as a preprocessing step for detection, which leads to suboptimal performance. Balancing the two tasks while enhancing detection-beneficial information remains challenging. In this paper, we present a detection-friendly union framework, termed UniCD, that simultaneously addresses both infrared NUC and UAV target detection tasks in an end-to-end manner. We first model NUC as a small number of parameter estimation problem jointly driven by priors and data to generate detection-conducive images. Then, we incorporate a new auxiliary loss with target mask supervision into the backbone of the infrared UAV target detection network to strengthen target features while suppressing the background. To better balance correction and detection, we introduce a detection-guided self-supervised loss to reduce feature discrepancies between the two tasks, thereby enhancing detection robustness to varying nonuniformity levels. Additionally, we construct a new benchmark composed of 50,000 infrared images in various nonuniformity types, multi-scale UAV targets and rich backgrounds with target annotations, called IRBFD. Extensive experiments on IRBFD demonstrate that our UniCD is a robust union framework for NUC and UAV target detection while achieving real-time processing capabilities.

## Dataset Download Link

The dataset used in our paper can be downloaded via the following link:

- Download Dataset Here -[Baidu Netdisk](<https://pan.baidu.com/s/1cgzAo8ZLIqplCV5tCIOldw?pwd=ujdm >) ,  [Google Drive(TODO)](<>)

## Online NUC Demo

We have developed an online demonstration website, allowing users to upload various non-uniform images for real-time processing. Our method does not require retraining and demonstrates excellent universal applicability across diverse scenarios.

- [Access the Online Demo Here](<>)[TODO]

Key Features:

- **No Retraining Required**: Immediately applicable to a wide range of infrared nonuniformity images.
- **Universal Applicability**: Outstanding performance across different  scenes.
- **Real-time Processing**: Supports real-time online demonstration for quick validation.







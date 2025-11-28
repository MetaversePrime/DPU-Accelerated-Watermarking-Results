# DPU-Accelerated-Watermarking-Results
Dataset of visual results showing a 192-bit invisible watermarking system guided by deep saliency maps. Watermarked and post-attack images are included for real-time embedded implementation studies.


This repository contains sample results generated from our saliency (visual attention)-guided stealth digital watermarking study. The repository includes original images, watermarked outputs embedded with 192-bit secret information, examples subjected to attacks such as JPEG, blurring, and scaling, and deep learning-based saliency maps. This data is being shared to support the reproducibility of this publication.

In this study, watermarking was performed using a deep learning-based embedding model and a fully hardware-accelerated inference module. The samples were taken from experiments conducted in both software and embedded platforms. The repository contains only experimental output samples; the model weights, training datasets, and codebase are not yet publicly available.


All Data Available Here :

https://drive.google.com/drive/folders/1ZKvzv2mjO1Xyim3kqlJwELNemnnW8mMV?usp=sharing


MobileNetv2
| Folder Name                       | Description                                                                                             |
| --------------------------------- | ------------------------------------------------------------------------------------------------------- |
| **watermarked_images_AI**         | Watermarked outputs generated using the AI-based autoencoder with MobileNetV2 saliency guidance         |
| **attacked_images_dct_qim_v2_a3** | DCT-QIM watermarking (α = 3), post-attack image samples                                                 |
| **attacked_images_dct_qim_v2_a4** | DCT-QIM watermarking (α = 4), post-attack image samples                                                 |
| **attacked_images_dct_qim_v2_a5** | DCT-QIM watermarking (α = 5), post-attack image samples                                                 |
| **attacked_images_dwt_qim_a3**    | DWT-QIM watermarking (α = 3), post-attack image samples                                                 |
| **attacked_images_dwt_qim_a4**    | DWT-QIM watermarking (α = 4), post-attack image samples                                                 |
| **attacked_images_dwt_qim_a5**    | DWT-QIM watermarking (α = 5), post-attack image samples                                                 |
| **saliency_results_kria**         | Real-time saliency maps (gray + overlay) produced by MobileNetV2 model running on Xilinx Kria KV260 DPU |
| **calib_images**                  | Calibration images used during Vitis AI INT8 quantization                                               |


FCN_ResNet-50

| Folder Name                                  | Description                                                                          |
| -------------------------------------------- | ------------------------------------------------------------------------------------ |
| **watermarked_images_AI**                    | Watermarked images generated using AI-based embedder guided by FCN-ResNet50 saliency |
| **attacked_images_dct_qim_v2_a3 / a4 / a5**  | DCT-QIM watermarking (α = 3/4/5), post-attack image samples                          |
| **attacked_images_dwt_qim_fcn_a3 / a4 / a5** | DWT-QIM watermarking (α = 3/4/5), post-attack image samples                          |
| **saliency_results_gray_fcn**                | Gray-scale saliency maps predicted by FCN-ResNet50                                   |
| **saliency_results_heatmap_fcn**             | Saliency visualization as heatmaps (FCN-based)                                       |
| **saliency_results_heatmap**                 | Overlay images: heatmap fused with source images (FCN-based)                         |
| **calib_images**                             | Calibration images for model quantization and benchmarking                           |


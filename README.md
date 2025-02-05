# Medical Image Segmentation Using U-Net++ for Glioma Detection

## Introduction
Gliomas are aggressive brain tumors that require precise detection for effective treatment. Multi-parametric MRI (mpMRI) scans provide essential information for tumor segmentation, aiding radiologists in diagnosis and treatment planning. This study leverages the BraTS dataset and implements an advanced U-Net++ deep learning model to segment tumor subregions, including necrotic core, edema, and enhancing tumor.

## Methodology
Dataset: The BraTS 2021 dataset is utilized, containing FLAIR, T1, T1CE, and T2 MRI modalities along with expert-annotated tumor segmentations.

Preprocessing: Images are normalized, padded to match dimensions, and multi-channel inputs are created.

Model: U-Net++, an advanced segmentation model with deep supervision and dense skip connections, is implemented.

Loss Function: Dice Loss is used to improve segmentation accuracy.

Training: The model is trained on multiple MRI cases using the Adam optimizer, and evaluated using Dice Score.

## Results
The model segments tumor subregions with low accuracy. The use of multi-modal MRI input and U-Net++ architecture enhances the detection of complex tumor structures. The validation loss demonstrates consistent learning over epochs, indicating effective model training. Furthermore, increasing the number of epochs can improve accuracy and refine segmentation predictions by allowing the model to learn more intricate tumor features and reduce misclassification.

## Conclusion
This study presents an efficient deep learning approach for glioma segmentation using U-Net++. The model effectively differentiates between tumor subregions, supporting automated medical diagnosis. Future work includes further optimizing hyperparameters and integrating clinical validation for real-world application.

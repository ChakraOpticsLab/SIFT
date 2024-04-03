# Signal Improved ultra-Fast Light-sheet Microscope (SIFT)
## SIFT initiatives
SIFT is a clear tisuue microscopic inititive that is capable to image centimeter scale tissue with isotropic submicron resolution. Our initiative involves the development of a tissue imaging pipeline that utilizes deep learning (DL) techniques for precise tissue boundary determination. Additionally, we have engineered a microscope that enhances signal-to-noise ratio (SNR) in images and accelerates frame acquisition rates by up to four times compared to existing ASLM (Advanced Single Lens Microscopy) microscopes.

![Temp](https://github.com/ChakraOpticsLab/SIFT/assets/157768359/8a25192d-367f-4d36-9e7b-acf71ca5dc91)

Fig. Optical path diagram of SIFT

## Deep learning based tissue boundary evaluation
![Temp](https://github.com/ChakraOpticsLab/SIFT/assets/157768359/4cd070c1-b3f4-403e-b631-8704f13ffb89)

Fig. Tissue imaging pipeline

This repository offers a tissue boundary classifier along with a pre-trained checkpoint. Users have the option to skip training the deep learning (DL) model and instead utilize our pre-trained checkpoint for identifying informative image sets. However, users also have the flexibility to train the network themselves for enhanced clarity if desired. Notably, the DL model is highly versatile and functional across various tissue types. The necessary dependencies are outlined in the 'Requirement.txt' file. By running only the 'Validationpy.py' file and ensuring correct directory placement, users can obtain a coordinate map delineating the tissue boundary. It's worth mentioning that the feature-based DL classifier significantly outperforms intensity-based thresholding methods in terms of efficiency and speed.

## Intensity based thresholding for tissue boundary evaluation
Additionally, we have created an intensity-based thresholding software capable of assessing tissue boundaries. However, it's important to note that the intensity threshold may not be universally applicable across different tissue types. Both the software and its required dependencies are specified in the 'Requirement.txt' file.

## Citation
If you find the work helpful in your resarch, please cite the following article:
Prince, M.N.H., Garcia, B., Henn, C. et al. Signal improved ultra-fast light-sheet microscope for large tissue imaging. Commun Eng 3, 59 (2024).
https://doi.org/10.1038/s44172-024-00205-4

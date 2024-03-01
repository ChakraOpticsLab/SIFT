# Signal Improved ultra-Fast Light-sheet Microscope (SIFT)
## SIFT initiatives
SIFT is a clear tisuue microscopic inititive that is capable to image centimeter scale tissue with isotropic submicron resolution. We developmed a tissue imaging pipeline where we determine the tissue boundary using deep learning (DL) based tissue informative image distinction. We also built a microsope which either enhances SNR to the images or speed up the frame acquisition rate by 4 fold compared to the existing ASLM microscope.

## SIFT implementation <video controls src="SIFT.mp4" title="Title"></video>

## Deep learning based tissue boundary evaluation

![Getting Started](./Temp.tif)

This repository provides the tissue boundary classifier with a trained checkpoint. User may chose not to train the DL model rather they can use our trained chekpoint to identify informative image sets. User may chose to train train the network by themselves for more clarity. Interestingly, DL model is quite functional for any kind of tissues. The required dependencies are mentioned in the 'Requirement.txt' file. User may need to run only'Validationpy.py' file keeping the directory right which will reture the coordinate map enclosing the tissue boundary. Feature based DL classifier is more efficient and faster compared to intensity based thresholding methos. 

## Intensity basedthresholding for tissue boundary evaluation
We also developed an intensity based thresholding software which is also able to evaluate the tissue boundary though the intensity threshold is not a generalized thing for different tissues. The software and the required dependencies are mentioned in the 'Requirement.txt' file.

## Citation
If you find the work helpful in your resarch or work, please cite the following paper:
M. N. H. Prince, B. Garcia, C. Henn, Y. Yi, E. A. Susaki, Y. Watakabe, T. Nemoto, K. A. Lidke, H. Zhao, I. S. Remiro, S. Liu, and T. Chakraborty, "Signal Improved ultra-Fast Light-sheet Microscope (SIFT) for large tissue imaging," 2023.05.31.543002 (2023).
doi: https://doi.org/10.1101/2023.05.31.543002

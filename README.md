# Surface deformation defect classification

__Surface deformation__ is a multi-factor, laser powder-bed fusion (LPBF) defect that cannot be avoided entirely using current monitoring systems. Distortion and warping, if left unchecked, can compromise the mechanical and physical properties resulting in a build with an undesired geometry. 
We propose a convolutional neural network-based solution to identify surface deformation defects from powder-bed. We printed thirteen bars with overhangs. We trained a __CNN__ and tested it with various model evaluation criteria. Our model is __99\% accurate__ in identifying the surface distortion from powder-bed images.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install required python libraries from the requirements.txt file.

```bash
pip install -r requirements.txt
```



## Notebooks Descriptions
In a nutshell, here is a brief description of what to expect in different Jupiter notebooks.
1. 1_Data_Collection.ipynb: Explains the image reading, cropping images, labelling images and storing the final datasets.
2. 2_Image_Augmentation.ipynb: Covers the various image data augmentation methods
3. 31_Image_Brightness_Edge_Detection_Binarisation.ipynb: Explains different image enhancement methods.
4. 3_Image_Enhancement_Examples.ipynb: Explains image histogram analysis, thresholding and Otsu binarization.
5. 4_Model_Training_CAD.ipynb: Trains a CNN using CAD labelling technique.
6. 5_Model_Training_XCT.ipynb: Trains a CNN using the XCT labelling approach.
7. 6_Model_Training_XCT-Debugging.ipynb: Explore the model's performance in predicting various sizes of pores.
8. 7_1_Hyperparameter_Tuning - Part1.ipynb: Prepares data for hyper-parameter tuning.
9. 7_2_Hyper_Parameter_Tuning - Part2.ipynb: Test CNN model with a range of hyper-parameters using hyperband tuner.
10. 7_3_Hyper_Parameter_Tuning - Part3.ipynb: Visualise and analyse hyper-parameter results.
11. 8_Model_training_XCT_Balanced_Data.ipynb: Final model trained on XCT labelled images and using balanced data after upsampling minority class via data augmentation. 


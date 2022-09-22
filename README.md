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
1. __1_Data_Preparation.ipynb:__ Reads the LPBF images, crops and labels them, and stores them as hdf5 file format.
2. __2_Sensor_Log_Files.ipynb:__ Explore and analyse different sensor files.
3. __3_Model_Building.ipynb:__ Trains a CNN Model.
4. __4_Model_Debugging.ipynb:__ Debuggs the model's internal working by visualising kernels and the CNN's feature maps of convolutional layers.
5. __5_Model_learning_rate_variation.ipynb:__ Final model trained on balanced data experimented with various learning rates of the optimisation algorithm, RMSprop.

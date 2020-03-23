# BraTS2018_Glioblastoma_whole_tumor_segmentation

Segmentation the brain Glioblastoma tumor with a UNET-like model which is implemented using Keras library. 

The code is implemented only for 2D images whcih are extracted from axial view of the Dicom data. 

The dicom data is released by MICCAI (https://www.med.upenn.edu/sbia/brats2018/data.html). I converted the data into 2D bitmap images (Axial view) and made 4-channel images (including T1, T2, FLAIR, T1contrast) each one with a binary mask image. You can download the converted data from: https://drive.google.com/open?id=1kIOVad8-O2WVtodMNGVozmerSJl9-X7-

The accuracy result is measured by Dice coefficient which is 0.85 for my training on segmenting the whole tumor.

# How to use:

The first cell (Getting_the_data.ipynb) is for installing necessary libraries and copying the data from google drive to the google colab system.
The second cell (Unzipping_the_data.ipynb) is for spliting the data into two category (test and train).
The third cell (Read_Data_And_Train) works as the the main program which you can train the data with different versions of unet-like models.

# P.S.
To start your training from a checkpoint, comment the fit_generator command (line 508) and uncomment the rest of the code (after line 516).

GoodLuck.
MeiH.

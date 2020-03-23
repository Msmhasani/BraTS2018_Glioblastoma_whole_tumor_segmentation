# BraTS2018_Glioblastoma_whole_tumor_segmentation
Segmentation the brain Glioblastoma tumor with a UNET-like model which is implemented using Keras library. 

The code is implemented only for 2D images whcih are extracted from axial view of the Dicom data. 

The dicom data is released by MICCAI (https://www.med.upenn.edu/sbia/brats2018/data.html). I convert the data into 2D images (Axial view) and made a 4-channel image (T1, T2, FLAIR, T1contrast) with a binary mask image. You can download the converted data from here: https://drive.google.com/open?id=1kIOVad8-O2WVtodMNGVozmerSJl9-X7-

The accuracy result is measured by Dice coefficient which is 0.85 for my training on segmenting the whole tumor.

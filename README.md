# BraTS
## Brain Tumor Segmentation in Magnetic resonance imaging (MRI) Using 3D BUNet model

## General info
There are two phases to this project: first, a diagnosis of brain tumors by segmenting combined structural mr images (T1, T1ce, T2, FLAIR) into three parts (ET, ED, NCR/NET), and second, a prognosis. <br />
The datasets were provided by University of Pennsylvania as part of the [BraTS challenge 2020](https://www.med.upenn.edu/cbica/brats2020/data.html). <b />

* Phase one: 
  * As part of phase one of this project, a 3D unet was designed with inputs of x, y, z, and d where x and y are the width and height of the image, z is the number of slices, and d represents four types of MRI images (t1, t1c, t2, flair). 
  * In order to reduce computational complexity of the model, using the data generator, a random subvolume of size (80, 80, 16, 4) is generated from the original sample (240, 240, 155, 4).



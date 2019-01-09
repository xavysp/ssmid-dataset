# Single Sensor Multispectral Images Dataset (SSMID)

<div align='center'>
<img src="images/bannerSSMID.jpg" width="800"/>
</div>

## Description

The SSMID is a set of three visible and near infrared datasets captured with two single sensor cameras (SSC).
The information acquired by such cameras was saved as RAW images. Images from the cameras are 
correctly registered as indicated [in the paper](http://www.cvc.uab.es/~asappa/publications/C__IEEE_IPTA_2017.pdf). 
Attempting to save as much as possible the whole of multispectral bands information, 
the SSMID datasets are packaged in a Matlab .mat file.

### 1.- Outdoor Multispectral Images with Vegetation (OMSIV) (OLD)
This dataset contains 533 nonregistered  Multispectral Images (MSI) with its respective ground truth for 
evaluation training stage). OMSIV.mat is a struct Matlab variable, it is organized as follow:
    
    rgb         | rgbn     |   name     |   rgb_imgs    |   rgbI_imgs   |   nir_imgs     
    ------------|----------|------------|---------------|---------------|------------
    256x256x3   |256x256x4 |images name |256x256x3 uint8|256x256x4 uint8|   256x256
    ---------------------------------------------------------------------------------
    There are 533 rows. The data type of each columns is double if it is not specified


#### Last OMSIV update
The former OMSIV version had 533 pair of images (visible and multispectral). The new actualization have  532 raw images, of that only 500 have remained after the "Registration" process. Therefore, if you are going to use the updated OMSIV ([Download OMSIV](https://drive.google.com/file/d/1KDi-JJLgMeM6iVN6WXbsAxSzL-_6lIJv/view?usp=sharing)) just 500 images will be found.
After the uncompression of omsiv.tar, you will find 4 folder [h5, raw, registered, restorations]. In the h5 folder you will find the images data in .h5 file, On the other hand, the raw folder has the same images as h5 but with .raw extension. The registered folder has 500 RGB and 500 respective RGB-NIR images. Those images are grouped in train and test folders. The train folder contains 400 images for the color correction using Deep Learning (DL) described in this [repo](https://github.com/xavysp/color_restorer). The remainder images are saved in the test folder for the  DL model testing.

### 2.- Outdoor Multispectral Images with no Vegetation (OMSINV)

OMSINV.mat is a Matlab struct  variable. It has 61 multispectral images  with its respective RGB ground truth images. This
variable is composed as follow:

    rgb         | rgbn     |   name     |   rgb_imgs    |   rgbI_imgs   |   nir_imgs     
    ------------|----------|------------|---------------|---------------|------------
    256x256x3   |256x256x4 |images name |256x256x3 uint8|256x256x4 uint8|   256x256
    ---------------------------------------------------------------------------------
    Thera are 61 rows. The data type of each columns is double if it is not specified
 
### 3.- One Scene Outdoor Multispectral Images (SSOMSI)
 The SSOMSI.mat matlab struct variable contains 150 MSI. It is composed by RGB with NIR influence and its respective  RGB ground truth images.
 The variable is organized as follow:
 
    rgb         | rgbn     |   name     |   rgb_imgs    |   rgbI_imgs   |   nir_imgs     
    ------------|----------|------------|---------------|---------------|------------
    256x256x3   |256x256x4 |images name |256x256x3 uint8|256x256x4 uint8|   256x256
    ---------------------------------------------------------------------------------
    Thera are 150 rows. The data type of each columns is double if it is not specified
 
 
## Download
 
 The entirely dataset (SSMID) can be downloaded from:
  [Click here to download](https://www.dropbox.com/s/qoh92yhrsb47pb8/SSMID.zip)
 
 Its  parts can be downloaded individually bellow:
 
<!-- OMSIV (in private mode yet)-->
[OMSIV (updated)](https://drive.google.com/file/d/1KDi-JJLgMeM6iVN6WXbsAxSzL-_6lIJv/view?usp=sharing)

[OMSIV (old)](https://drive.google.com/open?id=0B0givAGTBMIwUDJYejhsUFV0RVU)

<!--OMSINV (in private mode yet) -->
 [OMSINV](https://drive.google.com/open?id=0B0givAGTBMIwZzJrMm5YcXpWTzA)

[SSOMSI](https://drive.google.com/open?id=0B0givAGTBMIwNmxOb1BlVTVTdTg)

 
 

## Reference
We would appreciate if you cite our work when using the dataset:

    @INPROCEEDINGS{soria2017rgb-nirDataset,
    author={X. Soria and A. D. Sappa and A. Akbarinia},
    booktitle={2017 Seventh International Conference on Image Processing Theory, Tools and Applications (IPTA)},
    title={Multispectral single-sensor RGB-NIR imaging: New challenges and opportunities},
    year={2017},
    pages={1-6},
    keywords={Artificial neural networks;Cameras;Image color analysis;Image restoration;Sensitivity;Vegetation mapping;Color restoration;Multispectral images;Neural networks;RGB-NIR dataset;Single-sensor cameras},
    doi={10.1109/IPTA.2017.8310105},
    ISSN={2154-512X },
    month={Nov},
    organization={IEEE}}
    
  
## Contact
For any question please [Click here](https://xavysp.github.io/#contact) to contact us.
 
To open a RAW image you can find helps on [this repository](https://github.com/xavysp/rawImage_extractor) "as well as for dataset visualization".


<!-- Start of Simple-Counter Code -->
<a href="http://www.simple-counter.com/" target="_blank"><img src="http://www.simple-counter.com/hit.php?id=zrvfdff&nd=8&nc=3&bc=1" border="0" alt="Hit Counter"></a>
<!-- End of Simple-Counter Code -->

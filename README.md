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

#### Last OMSIV update
The former OMSIV version had 533 pair of images (visible and multispectral). The new actualization have  532 raw images, of that only 500 have remained after the "Registration" process. Therefore, if you are going to use the updated OMSIV ([Download OMSIV](https://drive.google.com/file/d/1KDi-JJLgMeM6iVN6WXbsAxSzL-_6lIJv/view?usp=sharing)) just 500 images will be found.
After the uncompression of omsiv.tar, you will find 4 folder [h5, raw, registered, restorations]. In the h5 folder you will find the images data in .h5 file, On the other hand, the raw folder has the same images as h5 but with .raw extension. The registered folder has 500 RGB and 500 respective RGB-NIR images. Those images are grouped in train and test folders. The train folder contains 400 images for the color correction using Deep Learning (DL) described in this [repo](https://github.com/xavysp/color_restorer). The remainder images are saved in the test folder for the  DL model testing.

<!-- Start of Simple-Counter Code -->
<a href="http://www.simple-counter.com/" target="_blank"><img src="http://www.simple-counter.com/hit.php?id=zrvfdff&nd=8&nc=3&bc=1" border="0" alt="Hit Counter"></a>
<!-- End of Simple-Counter Code -->

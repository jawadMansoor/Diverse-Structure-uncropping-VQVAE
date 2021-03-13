# Diverse Structure Inpainting

## Introduction
This repository is for the CVPR 2021 paper, "Generating Diverse Structure for Image Inpainting with Hierarchical VQ-VAE".

If our method is useful for your research, please consider citing.

<div align=center>
<img src="./intro.png" width="50%" height="50%">
</div>

*(Top) Input incomplete image, where the missing region is depicted in gray. (Middle) Visualization of the generated diverse structures. (Bottom) Output images of our method.*

## Installation
This code was tested with TensorFlow 1.12.0, CUDA 9.0, Python 3.6 and Ubuntu 16.04

Clone this repository：
```
git clone https://github.com/USTC-JialunPeng/Diverse-Structure-Inpainting.git
```

## Datasets
* [CelebA-HQ](https://github.com/tkarras/progressive_growing_of_gans): the 1024x1024 high-resolution face images from Growing GANs. 24183 for training, 2993 images for validation and 2824 images for testing.
* [Places2](http://places2.csail.mit.edu/): the challenge data from 365 scene categories. 8 Million images for training, 36K images for validation and 328K images for testing.
* [ImageNet](http://www.image-net.org/): the data from 1000 natural categories. 1 Million images for training and 50K images for validation.

## Training


## Testing

## Pre-trained Models
Download the pre-trained models using the following links and put them under `model_logs/` directory.

* `center_mask model`: [CelebA-HQ_center](https://drive.google.com/drive/folders/14Vskk15KUw6kYVkbyCJZw-7PUVhAiYqT) | [Places2_center](https://drive.google.com/drive/folders/1Dwi3HYC8ZDcqZvAnMQQUhMSKWOwkBTLJ) | [ImageNet_center](https://drive.google.com/drive/folders/1UanB-Yi4UkEma7tEsykjKKCKziS5Mb2Z)
* `random_mask model`: [CelebA-HQ_random](https://drive.google.com/drive/folders/1jLGVwWREwfGaKEzsr8f4IUqCCFANkFvG) | [Places2_random](https://drive.google.com/drive/folders/1h6tU-2P1j2DFAD42VntFS7XsKNRBI7__) | [ImageNet_random](https://drive.google.com/drive/folders/1ZNh9vjZGevCjUg-mF08pT6L3KZLo8MTL)

The **center_mask models** are trained with images of 256x256 resolution with center 128x128 holes. The **random_mask models** are trained with random regular and irregular holes.

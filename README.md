# VeIGAN: Vectorial Inpainting Generative Adversarial Networks for Depth Maps Object Removal

![VeIGAN GIF](https://github.com/nuneslu/VeIGAN/blob/master/examples/IVGif.gif)

## About
This code is based on the Generative Inpainting [CVPR 2018](https://arxiv.org/abs/1801.07892) paper and it's [repository](https://github.com/JiahuiYu/generative_inpainting).

Based on the Generative Inpainting network we proposed adaptations to deal with disparity images inpainting. Our results have been publish on [IV 2019](https://iv2019.org/) and on this repository we have the code used on this publication.

## Installation

To use this code, please follow the installation instructions from the original repository since de dependencies are the same.

## Usage

The directory _/training_data_ has the disparity images for the training and the _/data_flist_ contains the _.flist_ files wich list the images.

For training the command is:
```
python3 train.py
```

For testing use:
```
python3 test.py --image 'input_image' --mask 'removed_area_mask' --output 'output_image' --checkpoint_dir model_logs/'trained_model_dir'
```
For the paper all the train and test were made in a GeForce GTX 1080ti.

## VeIGAN Examples

Depth map object removal example and the respective 3D mesh reconstruction:

![Disparity Inpainting](https://github.com/nuneslu/VeIGAN/blob/master/examples/example.png)

## License

CC 4.0 Attribution-NonCommercial International

The software is for educaitonal and academic research purpose only.

## Citations

Please cite this work as follow:

{}

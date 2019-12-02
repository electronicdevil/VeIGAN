# VeIGAN: Vectorial Inpainting Generative Adversarial Networks for Depth Maps Object Removal

![VeIGAN GIF](https://github.com/nuneslu/VeIGAN/blob/master/examples/IVGif.gif)  

A video of our results can be seen in ![CityScapes Reconstruction](https://www.youtube.com/watch?v=0fQ3vPD88-w&feature=youtu.be)

## About
This code is based on the Generative Inpainting [[1](https://arxiv.org/abs/1801.07892)][[2](https://arxiv.org/abs/1806.03589)] papers and it's [repository](https://github.com/JiahuiYu/generative_inpainting).

Based on the Generative Inpainting network we proposed adaptations to deal with disparity images inpainting. Our results have been publish on [IV 2019](https://ieeexplore.ieee.org/document/8814157) and on this repository we have the code used on this publication.

## Installation

To use this code, please follow the installation instructions from the original [repository](https://github.com/JiahuiYu/generative_inpainting) since the dependencies are the same.

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

Object Removal from KITTI Images:

![KITTI Disparity Inpainting](https://github.com/nuneslu/VeIGAN/blob/master/examples/example.png)

Object Removal from CityScapes Images:

![CityScapes Disparity Inpainting](https://github.com/nuneslu/VeIGAN/blob/master/examples/spoiler_result.png)


## License

CC 4.0 Attribution-NonCommercial International

The software is for educational and academic research purpose only.

## Citations

Please cite this work as:

@INPROCEEDINGS{8814157,  
 author={L. P. N. {Matias} and M. {Sons} and J. R. {Souza} and D. F. {Wolf} and C. {Stiller}},  
 booktitle={2019 IEEE Intelligent Vehicles Symposium (IV)},  
 title={VeIGAN: Vectorial Inpainting Generative Adversarial Network for Depth Maps Object Removal},  
 year={2019},    
 pages={310-316},  
 doi={10.1109/IVS.2019.8814157},  
 ISSN={1931-0587},  
 month={June},  
}

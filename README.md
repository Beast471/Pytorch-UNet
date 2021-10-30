
# Pytorch U-Net 

A tunable implementation of U-Net in PyTorch.

## About U-Net
[U-Net](https://arxiv.org/abs/1505.04597) is a powerful encoder-decoder CNN architecture for semantic segmentation, developed by Olaf Ronneberger, Philipp Fischer and Thomas Brox.
This repository was created to

1 provide a reference implementation of 2D and 3D U-Net in PyTorch

2 allow fast prototyping and hyperparameter tuning by providing an easily parametrizable model.

Given model is tested on 3D [MICCAI BraTS dataset](https://drive.google.com/file/d/1XjN075TwlmT-N0ZqBC8JmmGfyGTU2SWi/view?usp=sharing)
It is found that given model performed extremely well for segmentation achieving the dice score of 97% on validation.

Along with this I have also tried to modify given architecture by introducing attention part in it. 
In first modification I have included [Squeeze and Excitation block](https://arxiv.org/abs/1709.01507v4) with unet and another combination was with [Project & Excite block](https://arxiv.org/abs/1906.04649).
Both implementations are giving promising results increasing dice score by 1% than simple UNets implementation.
(Implementation of each varient is given in saperate ipynb notebook)

Note: Implementation of SE-block and PE-block is for 3D data


## Model Inference (on BRaTS dataset) 

![image 1](https://github.com/Beast471/Pytorch-UNet/blob/master/asset/p1.png?raw=true){:height="50%" width="50%"}

![image 2](https://github.com/Beast471/Pytorch-UNet/blob/master/asset/p2.png?raw=true)
![image 3](https://github.com/Beast471/Pytorch-UNet/blob/master/asset/p3.png?raw=true)
![image 4](https://github.com/Beast471/Pytorch-UNet/blob/master/asset/p4.png?raw=true)


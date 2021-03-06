# Residual Networks Test
============================

Original Paper: "Deep Residual Learning for Image Recognition"(http://arxiv.org/abs/1512.03385) and "Identity Mappings in Deep Residual Networks"(http://arxiv.org/abs/1603.05027)

By [Kaiming He](http://research.microsoft.com/en-us/um/people/kahe/), [Xiangyu Zhang](https://scholar.google.com/citations?user=yuB-cfoAAAAJ&hl=en), [Shaoqing Ren](http://home.ustc.edu.cn/~sqren/), [Jian Sun](http://research.microsoft.com/en-us/people/jiansun/).

Microsoft Research Asia (MSRA).

## Introduction
This repository contains the models for testing resnet networks on cifar-10

50000 samples for training, batch size 250, 200 iterations for 1 epoch, 64000 iterations in total
10000 samples for testing, test batch size 100 and 100 test iterations
reduce learning rate after 32000 iters by factor of 10
then another factor of 10 after anohter 16000 iters

## Notes
### Data augmentation applied (please find the data augmentation fork in https://github.com/twtygqyy/caffe-augmentation): 

max_color_shift = 5

contrast_variation = 0.8 ~ 1.2

max_brightness_shift = 5 

zero-padding with 2 pixels for each side and crop with 32x32

## Result
Resnet-20: best model achieved 0.927 accuracy on test datasets for single round and single crop

Resnet-32: best model achieved 0.9364 accuracy on test datasets for single round and single crop

Resnet-56: best model achieved 0.9418 accuracy on test datasets for single round and single crop


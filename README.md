# Category-wise Attack

## Introduction
This repository contains the codes for Sparse Category Attack and Dense Category Attack.
The paper of Category-wise Attack has been submit to CVPR 2020.

#5843: Category-wise Attack: Transferable Adversarial Examples for Anchor Free Object Detection

## Implementation

### CenterNet

At first, you need to install the CenterNet and run successfully on MS-COCO and PascalVOC.
> [**Objects as Points**](http://arxiv.org/abs/1904.07850),    
> Xingyi Zhou, Dequan Wang, Philipp Krähenbühl,  
> https://github.com/xingyizhou/CenterNet

### Install SCA and DCA

Then, copy three *.py file into CenterNet-master/src/lib/detectors/.
and open CenterNet-master/src/lib/detectors/detector_factory.py, and change the 
> from .ctdet import CtdetDetector

into DCA
> from .ctdet_DCA import CtdetDetector

or SCA
> from .ctdet_SCA import CtdetDetector

Finally, run the CenterNet as before.

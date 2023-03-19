# mmrotate-dcfl
Official implementation for the CVPR23 paper: Dynamic Coarse-to-Fine Learning for Oriented Tiny Object Detection.
Coming soon!

## Introduction
DCFL is a learning framework for detecting oriented tiny objects.

**Abstract**: To be finished.

![demo image](figures/framework_final.png)

## Installation and Get Started
To be finished.

## Main Results

DOTA-v1.0

| Method |         Backbone         | AP50  | AP75  | mAP | Angle | lr schd | Aug  | Batch Size |                           Configs                          |  
| :-----: | :----------------------: | :---: | ----- | :---: | :-----: | :--: | :-------: |:-----:| :----------------------------------------------------------: | 
|RetinaNet-O| ResNet50 (1024,1024,200) | 69.17 | 36.71 | 39.33| le135  |   1x    |  Flipping   |     2      | [retinanet_obb_r50_dota1]() | 
|R3Det| ResNet50 (1024,1024,200) | 70.18 | 35.54 | 37.73| oc  |   1x    |  Flipping   |     2      | [r3det_oc_r50_dota1]() |
|ATSS-O| ResNet50 (1024,1024,200) | 73.12 | 43.66 | 43.04| le135  |   1x    |  Flipping   |     2      | [atss_le135_r50_dota1]() |
|S2A-Net| ResNet50 (1024,1024,200) | 74.12 | 43.14 | 42.33| le90  |   1x    |  Flipping   |     2      | [s2a_le90_r50_dota1]() | 
|DCFL| ResNet50 (1024,1024,200) | **74.26** | **47.55** | **45.07** | le135  |   1x    |  Flipping   |     2      |     [dcfl_r50_dota1]()      | 

DOTA-v2.0

| Method |         Backbone         | AP50  |  Angle | lr schd | Aug  | Batch Size |                           Configs                          | Speed |
| :-----: | :----------------------: | :---: | :-----: | :--: | :-------: |:-----:| :----------------------------------------------------------: | :--: |
|RetinaNet-O| ResNet50 (1024,1024,200) | 46.68 |  le135  |   1x    |  Flipping   |     2      | [retinanet_obb_r50_dota2]() | 20.8 FPS|
|R3Det w/ KLD| ResNet50 (1024,1024,200) | 47.26 |  le135  |   1x    |  Flipping   |     2      | [r3det_oc_r50_dota2]() | 16.2 FPS |
|ATSS-O| ResNet50 (1024,1024,200) | 49.57 |  le135  |   1x    |  Flipping   |     2      | [atss_le135_r50_dota2]() | - |
|S2A-Net| ResNet50 (1024,1024,200) | 49.86 |  le135  |   1x    |  Flipping   |     2      | [s2a_le135_r50_dota2]() | 18.9 FPS|
|DCFL| ResNet50 (1024,1024,200) | 51.57 | le135  |   1x    |  Flipping   |     2      |     [dcfl_r50_dota2]()      | 20.9 FPS |
|DCFL| ResNet101 (1024,1024,200) | **52.54** | le135  |   1x    |  Flipping   |     2      |     [dcfl_r101_dota2]()      | - |

## Visualization

## Citation
If you find this work helpful, please consider citing:
```bibtex
```
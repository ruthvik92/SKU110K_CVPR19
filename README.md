# SKU110K
Dataset and Codebase for CVPR2019 "Precise Detection in Densely Packed Scenes" [[Paper link]](https://arxiv.org/pdf/1904.00853.pdf)

<!---[alt text](figures/teaser_width.jpg)--->
<img src="figures/teaser_width.jpg" width="750">

A typical image in our SKU-110K, showing densely packed objects. (a) Detection results for the state-of-the-art RetinaNet[2], showing incorrect and overlapping detections, especially for the dark objects at the bottom which are harder to separate. (b) Our results showing far fewer misdetections and better fitting bounding boxes. (c) Zoomed-in views for RetinaNet[2] and (d) our method.

## Introduction
In our SKU-110K paper[1] we focus on detection in densely packed scenes, where images contain many objects, often looking similar or even identical, positioned in close proximity. These scenes are typically man-made, with examples including retail shelf displays, traffic, and urban landscape images. Despite the abundance of such environments, they are underrepresented in existing object detection benchmarks, therefore, it is unsurprising that state-of-the-art object detectors are challenged by such images.

We propose learning the Jaccard index with a soft Intersection over Union (Soft-IoU) network layer. This measure provides valuable information on the quality of detection boxes. Those detections can be represented as a Mixture of Gaussians (MoG), reflecting their locations and their Soft-IoU scores. Then, an Expectation-Maximization (EM) based method is then used to cluster these Gaussians into groups, resolving detection overlap conflicts. 

## To be added

## Method


## Dataset



## Qualitative Results
Add few results from the paper
<img src="qualitive_results.png" width="750">

## Dependencies

## Usage

## References
[1] Eran Goldman*, Roei Herzig*, Aviv Eisenschtat*, Jacob Goldberger, Tal Hassner, [Precise Detection in Densely Packed Scenes](https://arxiv.org/abs/1904.00853), 2019.

[2] Tsung-Yi Lin, Priyal Goyal, Ross Girshick, Kaiming He, Piotr Dollar, [Focal loss for dense object detection](https://arxiv.org/abs/1708.02002), 2018.


## Citation

```
@inproceedings{goldman2019dense,
 author    = {Eran Goldman and Roei Herzig and Aviv Eisenschtat and Jacob Goldberger and Tal Hassner},
 title     = {Precise Detection in Densely Packed Scenes},
 booktitle = {Proc. Conf. Comput. Vision Pattern Recognition (CVPR)},
 year      = {2019}
}
```

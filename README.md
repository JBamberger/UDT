# Unsupervised Deep Tracking
This repository includes the code for tracker UDT (conference version) and LUDT (journal version).

**Unsupervised Deep Representation Learning for Real-Time Tracking**   [paper link](https://arxiv.org/abs/2007.11984)

Ning Wang, Wengang Zhou, Yibing Song, Chao Ma, Wei Liu, and Houqiang Li 

Accepted by *IJCV 2020*

This is the journal version of our previous work. We make three changes: (1) We have extended the original multi-frame validation strategy. (2) We utilize an entropy-based image patch selection and HOG-based KCF tracker for data-preprocessing. (3) We visualized and analyzed the unsupervised feature representations. We have conducted more experiments on VOT2017/2018, LaSOT, and TrackingNet to justify our tracker.

**Unsupervised Deep Tracking**   [paper link](http://arxiv.org/abs/1904.01828)

Ning Wang, Yibing Song, Chao Ma, Wengang Zhou, Wei Liu, and Houqiang Li 

In *CVPR 2019*

### Pytorch Version 

Pytorch implementation of a simplified UDT is available at [UDT_pytorch](https://github.com/594422814/UDT_pytorch).

![](../master/UDT.png)

### Abstract
We propose an unsupervised visual tracking method in this paper. Different from existing approaches using extensive annotated data for supervised learning, our model is trained on large-scale unlabeled videos in an unsupervised manner. Our motivation is that a robust tracker should be effective in both the forward and backward ways, i.e., the tracker can forward localize the target object in successive frames and backtrace to its initial position in the first frame. We build our method on a Siamese correlation filter network, which is trained using raw videos without labels. Meanwhile, we propose a multiple-frame validation and a cost-sensitive loss to further facilitate the unsupervised learning. Without bells and whistles, our unsupervised tracker achieves the baseline accuracy of fully-supervised trackers, which require complete and accurate labels for training. Furthermore, unsupervised framework exhibits potential in leveraging unlabeled or weakly labeled data to further improve the tracking accuracy.

### Usage
Requirements: Matlab and [MatConvNet](http://www.vlfeat.org/matconvnet/install/).

Before running the code, you need to compile the matconvnet first.

For training and testing, please refer to the ```readme.md``` in the corresponding folder. 

### Acknowledge
Our baseline method is DCFNet and many parts of the code are from [DCFNet](https://github.com/foolwood/DCFNet).

### License
Licensed under an MIT license.

### Citation
If you find this work useful for your research, please consider citing our work and DCFNet:
```
@inproceedings{Wang_2019_Unsupervised,
    title={Unsupervised Deep Tracking},
    author={Wang, Ning and Song, Yibing and Ma, Chao and Zhou, Wengang and Liu, Wei and Li, Houqiang},
    booktitle={The IEEE Conference on Computer Vision and Pattern Recognition (CVPR)},
    year={2019}
}

@article{wang17dcfnet,
    Author = {Qiang Wang, Jin Gao, Junliang Xing, Mengdan Zhang, Weiming Hu},
    Title = {DCFNet: Discriminant Correlation Filters Network for Visual Tracking},
    Journal = {arXiv preprint arXiv:1704.04057},
    Year = {2017}
}
```

### Contact
If you have any questions, please feel free to contact wn6149@mail.ustc.edu.cn

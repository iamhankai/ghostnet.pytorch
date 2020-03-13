# GhostNet

This repo provides Pytorch implementation of CVPR 2020 paper [GhostNet: More Features from Cheap Operations](https://arxiv.org/abs/1911.11907). The TensorFlow implementation with pretrained model is available at [here](https://github.com/iamhankai/ghostnet).

### Requirements
The code was verified on Python3, PyTorch 1.0+.

### Usage
Usage example:
```
import torch
from ghost_net import ghost_net

model = ghost_net(width_mult=1.0)
input = torch.randn(32,3,224,224)
y = model(input)
print(y)
```

### Introduction of GhostNet

GhostNet: More Features from Cheap Operations. CVPR 2020. [[arXiv]](https://arxiv.org/abs/1911.11907)

By Kai Han, Yunhe Wang, Qi Tian, Jianyuan Guo, Chunjing Xu, Chang Xu.

- **Approach**

<div align="center">
   <img src="./fig/ghost_module.png" width="720">
</div>

- **Performance**

GhostNet beats other SOTA lightweight CNNs such as **MobileNetV3** and **FBNet**.

<div align="center">
   <img src="./fig/flops_latency.png" width="720">
</div>


## Citation
```
@inproceedings{ghostnet,
  title={GhostNet: More Features from Cheap Operations},
  author={Han, Kai and Wang, Yunhe and Tian, Qi and Guo, Jianyuan and Xu, Chunjing and Xu, Chang},
  booktitle={CVPR},
  year={2019}
}
```

# GaitSCM
Our code can be used in conjunction with the OpenGait framework.

OpenGait (https://github.com/ShiqiYu/OpenGait)

# Prerequires
- Python 3.7
- GPU
- Pytorch
- Torchvision


# Dataset
This model is trained on CASIA-B and OU-MVLP.

CASIA-B (http://www.cbsr.ia.ac.cn/english/Gait%20Databases.asp)

OU-MVLP (http://www.am.sanken.osaka-u.ac.jp/BiometricDB/GaitMVLP.html)

# Citation

@article{HUO2024103995,
title = {GaitSCM: Causal representation learning for gait recognition},
journal = {Computer Vision and Image Understanding},
volume = {243},
pages = {103995},
year = {2024},
issn = {1077-3142},
doi = {https://doi.org/10.1016/j.cviu.2024.103995},
url = {https://www.sciencedirect.com/science/article/pii/S1077314224000766},
author = {Wei Huo and Ke Wang and Jun Tang and Nian Wang and Dong Liang},
keywords = {Gait recognition, Global and local feature extractor, Disentangled representation learning, Causal representation learning},
abstract = {Gait recognition is a promising biometric technology that aims to identify the target subject via walking pattern. Most existing appearance-based methods focus on learning discriminative spatio-temporal representations from gait silhouettes. However, these methods pay less attention to probing the causality between identity factors and identity labels, which often mislead the model to learn gait representations that are susceptible to identity-irrelevant factors. In this paper, we attribute the cause that leads to the decline of model generalization under different external conditions to identity-irrelevant factors. We formulate the causalities among the identity factors, identity-irrelevant factors, and identity labels as a structural causal model (SCM). We accordingly propose a novel gait recognition framework named GaitSCM to learn covariate invariant gait representations, which is mainly composed of three components, including feature extraction module, feature disentanglement module, and backdoor adjustment. Specifically, we design a feature extractor with regard to the movement patterns of different body parts to learn fine-grained gait motion features, and then present a two-branch feature decoupling module to disentangle identity features and identity-irrelevant features with the aid of the classification confusion loss. To relieve the negative effect of identity-irrelevant factors, we develop a backdoor adjustment strategy to eliminate spurious associations between identity and identity-irrelevant features, which further facilitates the proposed framework to generate more powerful identity representations. Extensive experiments conducted on two public datasets validate the effectiveness of our method. The average Rank-1 can reach 93.2% and 90.4% on CASIA-B and OU-MVLP datasets, respectively, which verifies the superiority of GaitSCM. Source code is released at: https://github.com/HuoweiCode/GaitSCM.}
}



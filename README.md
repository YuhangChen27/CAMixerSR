## <div align="center"> <i>CAMixerSR</i>: Only Details Need More “Attention” </div>

<p align="center">
<a href="https://arxiv.org/abs/2402.19289" alt="arXiv">
    <img src="https://img.shields.io/badge/arXiv-2402.19289-b31b1b.svg?style=flat" /></a>
<a href="https://github.com/icandle/CAMixerSR/blob/main/LICENSE" alt="license">
    <img src="https://img.shields.io/badge/license-Apache--2.0-%23B7A800" /></a>
<a href="https://colab.research.google.com/gist/icandle/404a89adbc264294dd77edacfd80f3b2/camixersr.ipynb" alt="Colab">
    <img src="https://colab.research.google.com/assets/colab-badge.svg" /></a>
</p>

**Overview:** We propose ***CAMixerSR***, a new approach integrating *content-aware accelerating framework* and *token mixer design*, to pursue more efficient SR inference via assigning convolution for simple regions but window-attention for complex textures. It exhibits excellent generality and attains competitive results among state-of-the-art models with better complexity-performance trade-offs on large-image SR, lightweight SR, and omnidirectional-image SR.

<p align="center">
<img src="./figures/CAMixer.png" width=100% height=100% 
class="center">
</p>

This repository contains [PyTorch](https://pytorch.org/) implementation for ***CAMixerSR*** (CVPR 2024).

---

The main codes and pre-trained models have been uploaded. We are planning to replenish the README of CAMixerSR in a few weeks.
 
Requirements
---
- [PyTorch >= 1.8](https://pytorch.org/) 
- [BasicSR == 1.4.2](https://github.com/XPixelGroup/BasicSR/blob/master/INSTALL.md)
- [einops](https://github.com/arogozhnikov/einops)
  
### Installation
```
pip install -r requirements.txt
```


Datasets
---
#### Large-Image SR

&emsp;*Training*: [DIV2K](https://data.vision.ee.ethz.ch/cvl/DIV2K/).

&emsp;*Testing*: [F2K](https://drive.google.com/file/d/1jubeKExUrUE-VKpiTx9AAUVodJZvdkBC/view?usp=drive_link), [Test2K](https://drive.google.com/file/d/1HQtKhWrVSrUNh0bcka57BlhbZWCCB649/view?usp=drive_link), [Test4K](https://drive.google.com/file/d/1yBCRPHzcNzSX6xLsgFjgJuRlcVJWA4ZD/view?usp=sharing), [Test8K](https://drive.google.com/file/d/1CXVF61888zQRP8gkPGoX5LFD9IBcV-Sl/view?usp=drive_link) ([Google Drive](https://drive.google.com/drive/folders/1wSdB9GUa2IsYe5S8pHV-7d8dYdZA2wDp?usp=drive_link)/Baidu Netdisk).

#### Lightweight SR

&emsp;*Training*: [DIV2K](https://data.vision.ee.ethz.ch/cvl/DIV2K/) or [DF2K](https://openmmlab.medium.com/awesome-datasets-for-super-resolution-introduction-and-pre-processing-55f8501f8b18).

&emsp;*Testing*: Set5, Set14, BSD100, Urban100, Manga109 (Download at [Google Drive](https://drive.google.com/file/d/1SbdbpUZwWYDIEhvxQQaRsokySkcYJ8dq/view?usp=sharing)/Baidu Netdisk).

#### Omni-Directional-Image SR

&emsp;*Training*: [lau dataset](https://drive.google.com/file/d/1FjEzVh7-0swloClKCVnctUS8Wmlz3Ibv/view?usp=drive_link).

Acknowledgments
---
We would thank *[BasicSR](https://github.com/XPixelGroup/BasicSR)*, *[ClassSR](https://github.com/XPixelGroup/ClassSR)*, and *[OSRT](https://github.com/Fanghua-Yu/OSRT)* for their enlightening work!

Citation
---
```
@article{wang2024camixersr,
  title={CAMixerSR: Only Details Need More ``Attention"},
  author={Wang, Yan and Liu, Yi and Zhao, Shijie and Li, Junlin and Zhang, Li},
  journal={arXiv preprint arXiv:2402.19289},
  year={2024}
}
```


# RealMat: Realistic Materials with Diffusion and Reinforcement Learning

### [Paper](https://arxiv.org/pdf/2509.01134) | [Project Page](https://pedrovfigueiredo.github.io/)

This is the official implementation of the paper "RealMat: Realistic Materials with Diffusion and Reinforcement Learning"

<p align="center">
<img src="assets/teaser.gif" width="800px"/> <br/>
<strong>RealMat</strong> generates diverse realistic materials.
</p>

## Abstract
<p align="justify">
Generative models for high-quality materials are particularly desirable to make 3D content authoring more accessible. However, the majority of material generation methods are trained on synthetic data. Synthetic data provides precise supervision for material maps, which is convenient but also tends to create a significant visual gap with real-world materials. Alternatively, recent work used a small dataset of real flash photographs to guarantee realism, however such data is limited in scale and diversity. To address these limitations, we propose <strong>RealMat</strong>, a diffusion-based material generator that leverages realistic priors, including a text-to-image model and a dataset of realistic material photos under natural lighting. In <strong>RealMat</strong>, we first finetune a pretrained Stable Diffusion XL (SDXL) with synthetic material maps arranged in 2 × 2 grids. This way, our model inherits some realism of SDXL while learning the data distribution of the synthetic material grids. Still, this creates a realism gap, with some generated materials appearing synthetic. We propose to further finetune our model through reinforcement learning (RL), encouraging the generation of realistic materials. We develop a realism reward function for any material image under natural lighting, by collecting a large-scale dataset of realistic material images. We show that this approach increases generated materials' realism compared to our base model and related work.
</p>

## News
- **2025.10.02**: Repo is released.

## TODO List
- [ ] Code Release

## Citation
If our work is useful for your research, please consider citing:
```
@article{zhou2025realmat,
  title={RealMat: Realistic Materials with Diffusion and Reinforcement Learning},
  author={Zhou, Xilong and Figueiredo, Pedro and Ha{\v{s}}an, Milo{\v{s}} and Deschaintre, Valentin and Guerrero, Paul and Hu, Yiwei and Kalantari, Nima Khademi},
  journal={arXiv preprint arXiv:2509.01134},
  year={2025}
}
```
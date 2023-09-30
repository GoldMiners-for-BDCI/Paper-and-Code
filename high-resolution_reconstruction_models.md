
## Ideas
- SRCNN - ECCV2014
- ESPCN - CVPR2016
- DRCN - CVPR2016
- RED - NIPS2016
- FSRCNN - ECCV2016
- VDSR - CVPR2016
- EDSR - CVPRW2017
- ▶️:SRGAN (SRRestnet) - CVPR2017
- DRRN - CVPR2017
- SRDenseNet - ICCV2017
- CARN - ECCV2018
- FALSR - >2018
- MMSDB-SR - 2018
- Improved FSRCNN - 2019
- MFSCSR - 2020
- ▶️:ESRGAN - 2020
- GLRDN - 2022
- LRR-CED - 2022
- real-ESRGAN - 2022
- T-GAN - 2022
- ✔️MARDGAN - 2023
- sparsity regularization and deep residual-learned priors - 2023
- ~~RawHDR - 2023 ICCV~~
- Score-Based Generative Models for PET Image Reconstruction - 2023
- PADUT - 2023 ICCV
- SDLFormer - 2023
- TransMRSR - 2023
- FA-VAE - 2023CVPR
- DRSformer - 2023CVPR
- Raw Image Reconstruction with Learned Compact Metadata - 2023CVPR


Checkout : [ZHIHU](https://zhuanlan.zhihu.com/p/263008440), [PaperWithCode](https://paperswithcode.com/task/image-reconstruction/latest)


## 2023
### (MARDGAN)(not implemented) Image super-resolution reconstruction based on multi-scale dual-attention

Paper:
- [MARDGAN](https://www.tandfonline.com/doi/full/10.1080/09540091.2023.2182487)

Problems solved: 
- missing details, distorted natural texture, blurred details and too smooth after image reconstruction.

Model:
- Multi-scale Dual-Attention based Residual Dense Generative Adversarial Network (MARDGAN)
- channel and spatial attention block (CSAB)
- enhanced residual dense block (ERDB) 

![](blob:https://qv6rfojn7rl.feishu.cn/84cf0090-5edc-4cad-b81f-d77d9e1cc13c)

1. Feature extraction (CNN + CSAB + ERDB)
2. Feature Diffusion (split + concat)
3. Skip connection (GRL)
4. Upsampling (conv, organizing)
5. Discriminator for testing


![Discriminator](blob:https://qv6rfojn7rl.feishu.cn/b6bc9493-373a-4598-900c-c6165f5ccd3f)
![CSAB](blob:https://qv6rfojn7rl.feishu.cn/bcf1df6d-8c60-47ad-945a-900121509428)
![channel attention, spatial attention](blob:https://qv6rfojn7rl.feishu.cn/ae6c5983-3e1d-4dcc-9718-26d681d01e57)
![SPP](blob:https://qv6rfojn7rl.feishu.cn/a3cab524-f472-4f1a-9f74-d3a2f4de6cbe)

![ERDB](blob:https://qv6rfojn7rl.feishu.cn/93e006da-9494-4632-a032-d2f9cf9fb928)

Experiments:
![](blob:https://qv6rfojn7rl.feishu.cn/c6e2a243-713f-49d7-b3b0-aba991b8cf61)



### (RawHDR)(Deprecated) High Dynamic Range Image Reconstruction from a Single Raw Image

> Deprecated, the proposed method is designed for recovery from high exposures rather than high-resolution reconstructing from blurred images. Raw images are required as well. 

Problems solved:
- retrieve extremely high dynamic range scenes from such limited bit-depth data
- single exposure HDR reconstruction

Model:
![](blob:https://qv6rfojn7rl.feishu.cn/80ad52b1-adc3-4e9e-bd95-89c98a6940c1)

1. Learn exposure masks through mask estimation module
2. Dual intensity guidance
3. Global spatial guidance (transformer-based)



### (SRGAN) Photo-Realistic Single Image Super-Resolution Using a Generative Adversarial Network

Github:
- SRGAN

> TBC



### (ESRGAN) Enhanced Super-Resolution Generative Adversarial Networks

Github: 
- real-ESRGAN
- ESRGAN

Paper:
- ESRGAN

Problems solved:
- SR-GAN : generating realistic textures with unpleasant artifacts
- Enhance visual quality
- Improved SRGAN

Model:
![](blob:https://qv6rfojn7rl.feishu.cn/5e3ac538-b5fe-4612-8a80-65b6598e0ff6)

> TBC



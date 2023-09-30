
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

![Architecture](https://www.tandfonline.com/cms/asset/b90766fc-2220-47c1-a822-7e04f1801c57/ccos_a_2182487_f0001_oc.jpg)

1. Feature extraction (CNN + CSAB + ERDB)
2. Feature Diffusion (split + concat)
3. Skip connection (GRL)
4. Upsampling (conv, organizing)
5. Discriminator for testing


![Discriminator](https://www.tandfonline.com/cms/asset/6befdf16-f013-40ce-ae77-832b5869ed7f/ccos_a_2182487_f0002_oc.jpg)
![CSAB](https://www.tandfonline.com/cms/asset/fcb4012c-4e82-42df-abe2-ee606eee342c/ccos_a_2182487_f0003_oc.jpg)
![channel attention, spatial attention](https://www.tandfonline.com/cms/asset/bdbdf5f5-26bc-44a9-8a9b-e4c635509df8/ccos_a_2182487_f0004_oc.jpg)
![SPP](https://www.tandfonline.com/cms/asset/17a63f9b-ea86-467b-b5f5-f90583225e3d/ccos_a_2182487_f0005_oc.jpg)

![ERDB](https://www.tandfonline.com/cms/asset/0b7a7375-5631-4034-9ec4-1acb738b9945/ccos_a_2182487_f0006_oc.jpg)

Experiments:
![](https://www.tandfonline.com/cms/asset/759fda33-8d93-4432-b1a4-4bcc7268b32c/ccos_a_2182487_f0012_oc.jpg)



### (RawHDR)(Deprecated) High Dynamic Range Image Reconstruction from a Single Raw Image

> Deprecated, the proposed method is designed for recovery from high exposures rather than high-resolution reconstructing from blurred images. Raw images are required as well. 

Problems solved:
- retrieve extremely high dynamic range scenes from such limited bit-depth data
- single exposure HDR reconstruction

Model:
![architecture](https://qv6rfojn7rl.feishu.cn/docx/YbmOdbzpCoFN2ixAlLxcUzven4e#KUiPdxnGIojhyDxV8fociRKSnNg)

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
![](https://esrgan.readthedocs.io/en/latest/_images/architecture.png)

> TBC



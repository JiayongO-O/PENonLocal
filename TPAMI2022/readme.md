## [Boosting Photon-Efficient Image Reconstruction With A Unified Deep Neural Network](https://ieeexplore.ieee.org/document/9864284)

[Jiayong Peng](https://scholar.google.com/citations?user=cXdZl0wAAAAJ&hl=en), [Zhiwei Xiong](https://scholar.google.com/citations?user=Snl0HPEAAAAJ&hl=en), [Hao Tan](https://ieeexplore.ieee.org/author/37088634970), [Xin Huang](https://quantum.ustc.edu.cn/web/en/node/480), [Zheng-Ping Li](https://quantum.ustc.edu.cn/web/en/node/694), [Feihu Xu](https://scholar.google.ca/citations?user=-EZOdMIAAAAJ&hl=en)

----

#### 1. Introduction

Photon-efficient imaging, which captures 3D images with single-photon sensors, has enabled a wide range of applications. However, two major challenges limit the reconstruction performance, i.e., the low photon counts accompanied by low signal-to-background ratio (SBR) and the multiple returns. In this paper, we propose a unified deep neural network that, for the first time, explicitly addresses these two challenges, and simultaneously recovers depth maps and intensity images from photon-efficient measurements. Starting from a general image formation model, our network is constituted of one encoder, where a non-local block is utilized to exploit the long-range correlations in both spatial and temporal dimensions of the raw measurement, and two decoders, which are designed to recover depth and intensity, respectively. Meanwhile, we investigate the statistics of the background noise photons and propose a noise prior block to further improve the reconstruction performance. The proposed network achieves decent reconstruction fidelity even under extremely low photon counts / SBR and heavy blur caused by the multiple-return effect, which significantly surpasses the existing methods. Moreover, our network trained on simulated data generalizes well to real-world imaging systems, which greatly extends the application scope of photon-efficient imaging in challenging scenarios with a strict limit on optical flux.

#### 2. Usage

- Install requirements
  
  `pip install -r requirements.txt`

- Download NYU V2 raw data and build train and test data
- Edit the corresponding parameters in `./training/config.ini`

- Run the main train file

  `python ./training/main.py`

- Edit the corresponding parameters in `./testing/config.ini`

- Run the main test file

  `python ./testing/main.py`


#### 3. Citation

If you find the code useful in your research, please consider citing:
```
@article{peng2022boosting,
  title={Boosting Photon-Efficient Image Reconstruction with A Unified Deep Neural Network},
  author={Peng, Jiayong and Xiong, Zhiwei and Tan, Hao and Huang, Xin and Li, Zheng-Ping and Xu, Feihu},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
  year={2022},
  publisher={IEEE}
}
```
























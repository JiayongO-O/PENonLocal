## [Photon-Efficient 3D Imaging with A Non-Local Neural Network](https://www.ecva.net/papers/eccv_2020/papers_ECCV/html/5471_ECCV_2020_paper.php)

#### **ECCV2020** [Spotlight]

[Jiayong Peng](https://scholar.google.com/citations?user=cXdZl0wAAAAJ&hl=en), [Zhiwei Xiong](https://scholar.google.com/citations?user=Snl0HPEAAAAJ&hl=en), [Xin Huang](https://quantum.ustc.edu.cn/web/en/node/480), [Zheng-Ping Li](https://quantum.ustc.edu.cn/web/en/node/694), [Dong Liu](https://scholar.google.com/citations?user=lOWByxoAAAAJ&hl=en), [Feihu Xu](https://scholar.google.ca/citations?user=-EZOdMIAAAAJ&hl=en)

----

#### 1. Introduction

Photon-efficient imaging has enabled a number of applications relying on single-photon sensors that can capture a 3D image with as few as one photon per pixel. In practice, however, measurements of low photon counts are often mixed with heavy background noise, which poses a great challenge for existing computational reconstruction algorithms. In this paper, we first analyze the long-range correlations in both spatial and temporal dimensions of the measurements. Then we propose a non-local neural network for depth reconstruction by exploiting the long-range correlations. The proposed network achieves decent reconstruction fidelity even under photon counts (and signal-to-background ratio, SBR) as low as 1 photon/pixel (and 0.01), which significantly surpasses the state-of-the-art. Moreover, our non-local network trained on simulated data can be well generalized to different real-world imaging systems, which could extend the application scope of photon-efficient imaging in challenging scenarios with a strict limit on optical flux.

#### 2. Usage

- Install requirements
  
  `pip install -r requirements.txt`

- Download NYU V2 raw data and build train and test data
- edit the corresponding parameters in `./training/config.ini`

- run the main train file

  `python ./training/main.py`

- edit the corresponding parameters in `./testing/config.ini`

- run the main test file

  `python ./testing/main.py`


#### 3. Citation

If you find the code useful in your research, please consider citing:
```
@inproceedings{peng2020photon,
  title={Photon-efficient 3d imaging with a non-local neural network},
  author={Peng, Jiayong and Xiong, Zhiwei and Huang, Xin and Li, Zheng-Ping and Liu, Dong and Xu, Feihu},
  booktitle={Computer Vision--ECCV 2020: 16th European Conference, Glasgow, UK, August 23--28, 2020, Proceedings, Part VI 16},
  pages={225--241},
  year={2020},
  organization={Springer}
}
```
























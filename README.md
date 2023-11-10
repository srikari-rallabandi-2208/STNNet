
# Improved STTNet
## Introduction

In the realm of computer vision, multi-object tracking in crowded scenes stands as a pivotal challenge with diverse applications, from surveillance systems to autonomous vehicles. Existing tracking methods such as video surveillance for crowd control [26] and public safety [11] often face difficulties in precisely associating noisy object detections and maintaining consistent labels across frames. To address these challenges, this paper presents ’Improved STNNet’, an advanced framework for online Multi-Object Tracking (MOT). Building upon the foundational STNNet architecture, our improved model refines the decision-making process by incorporating deep reinforcement learning techniques. By formulating the online MOT problem as a Markov Decision Process (MDP), Improved STNNet learns a sophisticated policy for data association. Notably, the framework adeptly handles complexities such as object birth/death and appearance/disappearance, treating them as state transitions within the MDP. Through rigorous experimentation on benchmark datasets, including the MOT Challenge, our proposed Improved STNNet demonstrates superior performance, outperforming existing methods in challenging, crowded scenarios. The study not only provides compelling evidence of the efficacy of our approach but also opens avenues for advancing real-time video analysis applications, especially in dynamic, crowded environments.Some recent efforts [2, 4, 16, 22, 23, 25] have devoted to construct datasets for crowd counting. For density map estimation, we used the dataset constructed and provided by STNNET [18] upong which this paper is extensively based upon.

## Dataset
We have extensively used the Datasets used in STNNet, as well as using the datasets from other sources like ShanghaiTech Crowd Counting Dataset. It consists of 1198 annotated crowd images. The dataset is divided into two parts, Part-A containing 482 images and Part-B containing 716 images. Part-A is split into train and test subsets consisting of 300 and 182 images, respectively. Part-B is split into train and test subsets consisting of 400 and 316 images. Each person in a crowd image is annotated with one point close to the center of the head. In total, the dataset consists of 330,165 annotated people. Images from Part-A were collected from the Internet, while images from Part-B were collected on the busy streets of Shanghai.

### ECCV2020 Challenge

The VisDrone 2020 Crowd Counting Challenge requires participating algorithms to count persons in each frame. The challenge will provide 112 challenging sequences, including 82 video sequences for training (2,420 frames in total), and 30 sequences for testing (900 frames in total), which are available on the download page. We manually annotate persons with points in each video frame. 

DroneCrowd (1.03 GB): [BaiduYun](https://pan.baidu.com/share/init?surl=llJZJMi2L5oUQvj31iBlfg)(code: h0j8)| [GoogleDrive](https://drive.google.com/file/d/1HY3V4QObrVjzXUxL_J86oxn2bi7FMUgd/view?usp=sharing) 

### DroneCrowd (Full Version)
This full version consists of 112 video clips with 33,600 high resolution frames (i.e., 1920x1080) captured in 70 different scenarios.  With intensive amount of effort, our dataset provides 20,800 people trajectories with 4.8 million head annotations and several video-level attributes in sequences.  

DroneCrowd [BaiduYun](https://pan.baidu.com/s/1hjXoVZJ16y9Tf7UXcJw3oQ)(code:ml1u)| [GoogleDrive](https://drive.google.com/drive/folders/1EUKLJ1WmrhWTNGt4wFLyHRfspJAt56WN?usp=sharing) 

## Code

[Space-Time Neighbor-Aware Network (STNNet-pytorch)](https://github.com/srikari-rallabandi-2208/STNNet/tree/master/STNNet)

[Space-Time Multi-Scale Attention Network (STANet-pytorch)](https://github.com/srikari-rallabandi-2208/STNNet/tree/master/STANet)

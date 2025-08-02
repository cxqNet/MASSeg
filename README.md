# CVPR 2025 - MOSE Track of the 4th PVUW challenge

# MASSeg : Multi-scale-Aware Segmentation Network for Complex Video Object Segmentation


<p align="middle">
    <img src="fig/CVPRpic.jpeg" style="width:800px; height:250px;">
</p>

### 🏅 Paper on [[arXiv]](https://arxiv.org/abs/2504.10254)   | 🏛️ **[[ MOSE Homepage ]](https://henghuiding.github.io/MOSE/)**  


**Author:** Xuqiang Cao, Linnan Zhao, Jiaxuan Zhao, Fang Liu, Puhua Chen, Wenping Ma 

# Introduce
**MASSeg** is our 2nd place solution to the CVPR 2025 PVUW MOSE Challenge. It enhances a segmentation framework with mask scaling, MOSE-specific data augmentation, and the MOSE+ dataset, achieving a **J&F** score of **0.8628**. 
<p align="middle">
    <img src="fig/主框架3.png" style="width:800px; height:300px;">
</p>

# Installation 
MASSeg needs to be installed first before use. The code requires `python>=3.10`, as well as `torch>=2.5.1` and `torchvision>=0.20.1`. Please follow the instructions [here](https://pytorch.org/get-started/locally/) to install both PyTorch and TorchVision dependencies. You can install MASSeg on a GPU machine using:

### Clone this repository

   ```bash
   git clone --depth 1 https://github.com/cxqNet/MASSeg.git  && cd MASSeg

   pip install -e .
   ```
# Getting Started
### Datasets Preparation
We integrated a new dataset "MOSE+" to improve the performance of the model in the training phase
The dataset "MOSE+" can be downloaded from this link of [BaiduPan](https://pan.baidu.com/s/1MD66adP51ury-16_ukB6uw?pwd=mc43). Please place it in the `data` folder and confirm the file structure as follows:
```
MASSeg/
    |- data
        |- MOSE+
           |- JPEGImages
           |- Annotations
           |- moseplus.txt
    |- Training
    |- tools
    |- ...
```
### Download Pretrained Weights
We provide the pretrained model weights used in the Track. You can download them via the link below:  

🔗 Baidu Netdisk Download Link: [[BaiduPan]](https://pan.baidu.com/s/1qCTcd0531ea2uYupUb7OEw?pwd=jhgw)

After downloading, please place the weights in the following directory:

```
MASSeg/
    |- checkpoints/
        │- mass_seg_mose.pth
```

# MOSE Challenge Organizers :

<table align="center" cellspacing="10">
  <tr align="center">
    <td width="160px">
      <img src="fig/HenghuiDing.jpg" width="100"><br>
      <a href="https://henghuiding.github.io/"><b>Henghui Ding</b></a><br>
      <i>Primary Organizer<br>Fudan University</i>
    </td>
    <td width="60px"></td> <!-- 空隔 -->
    <td width="160px">
      <img src="fig/LiuChang.jpg" width="100"><br>
      <a href="https://scholar.google.com/citations?hl=en&authuser=1&user=XlQP0GIAAAAJ"><b>Chang Liu</b></a><br>
      <i>Primary Organizer<br>Nanyang Technological University</i>
    </td>
  </tr>
</table>

<br>


<table align="center" cellspacing="10">
  <tr align="center">
    <td width="160px">
      <img src="fig/ShutingHe.jpg" width="100"><br>
      <a href="https://heshuting555.github.io/"><b>Shuting He</b></a><br>
      <i>Nanyang Technological University</i>
    </td>
    <td width="40px"></td>
    <td width="160px">
      <img src="fig/JiangXudong.jpg" width="100"><br>
      <a href="https://personal.ntu.edu.sg/exdjiang/"><b>Xudong Jiang</b></a><br>
      <i>Nanyang Technological University</i>
    </td>
    <td width="40px"></td>
    <td width="160px">
      <img src="fig/PhilipTorr.jpg" width="100"><br>
      <a href="https://www.robots.ox.ac.uk/~phst/"><b>Philip H.S. Torr</b></a><br>
      <i>University of Oxford</i>
    </td>
    <td width="40px"></td>
    <td width="160px">
      <img src="fig/SongBai.jpg" width="100"><br>
      <a href="https://songbai.site/"><b>Song Bai</b></a><br>
      <i>ByteDance</i>
    </td>
  </tr>
</table>

## References
- We especially thank the authors of **[MOSE](https://github.com/henghuiding/MOSE-api)** for providing a valuable and challenging dataset, which significantly advances research in complex video object segmentation.  
- We also appreciate the open-source contributions of [Sam2](https://github.com/facebookresearch/sam2) and [Cutie](https://github.com/hkchengrex/Cutie), whose frameworks and ideas greatly inspired and supported our work.



# Learning Tracking Representations via Dual-Branch Fully Transformer Networks 
## DualTFR
:star: We achieves the runner-ups for both VOT2020ST (short-term) and RT(real-time). The variants of DualTFR take 3rd/4th places of VOT2020RT and 5th places of VOT2020ST
### For VOT21 challenge model weight download:

We provide the models of Five trackers *SAMN*, *SAMN_DiMP*, *DualTFR*, *DualTFRst*, *DualTFRon* here.

Note that the *AlphaRefine* (https://github.com/MasterBin-IIAU/AlphaRefine) model 
and *SuperDiMP* (https://github.com/visionml/pytracking) model are the same
with the original author.

| Tracker        |      model quantity    |  model name    | 
|:--------------:|:----------------:|:----------------:|
| SAMN |   1  | SAMN.tar |
| SAMN_DiMP |   2  | super_dimp.pth.tar,  SAMN.tar |
| DualTFR |  2   | DualTFR.tar,  ar.pth.tar |
| DualTFRst |  2   | DualTFRst.tar,  ar.pth.tar  |
| DualTFRon |  2   | DualTFRon.tar,  ar.pth.tar  |

Models can be downloaded from BaiduNetDisk or GoogleDrive:

BaiduNetDisk:

https://pan.baidu.com/s/1RHA7HVlXtNEzYPGIjJbQ-g (sruh) 

GoogleDrive: 

https://drive.google.com/drive/folders/1Z61_mfh2vwzqDxejt5idBOgYhWOCZOr5?usp=sharing

## Code will be released soon.

We present a simple Siamese-like Dual-branch network based on solely Transformer networks to learn about tracking features.  Given a template and a search image, we divide them into non-overlapping image patches and extract a feature vector for each based on its matching results with others within an attention window.  Then for each token, we estimate whether it contains the target object and the corresponding size. The prominent advantage of the approach is that **the features are learned from matching, and ultimately, for matching**. So the features are aligned with the subsequent object tracking task. The method achieves comparable results comparing to the best-performing methods which first use CNN to extract features and then use Transformer to fuse them. Without bells and whistles, it outperforms the state-of-the-art methods on GOT-10k and VOT2020 benchmarks. In addition, the method achieves real-time inference speed (about 40 fps).

## Acknowledgments
* Thanks for the great [PyTracking](https://github.com/visionml/pytracking) Library, which helps us to quickly implement our ideas.
* We use the implementation of the Swin Transformer from the official repo [https://github.com/microsoft/Swin-Transformer](https://github.com/microsoft/Swin-Transformer).  

## Contacts
* Fei Xie, School of Automation, Southeast University, China, 372998044@qq.com, wechat: 372998044


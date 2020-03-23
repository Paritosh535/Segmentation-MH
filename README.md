# Segmentation-MH

1. Install global dependencies

    - python3.6


2. Clone repository

Clone repo to local folder.

    $ git clone https://github.com/Paritosh535/Segmentation-MH.git

3. Install dependencies

Install Python dependencies

    pip install -r config/req.pip  # for Python


## Multi-Human Parsing (MHP) v2.0 Dataset
<img src="https://github.com/ZhaoJ9014/Multi-Human-Parsing_MHP/blob/master/Figures/Fig3.png" width="1000px"/>


<img src="https://github.com/ZhaoJ9014/Multi-Human-Parsing_MHP/blob/master/Figures/Fig4.png" width="1000px"/>



- Statistics: The MHP v2.0 dataset contains 25,403 images, each with at least two persons (average is 3). We randomly choose 5,000 images and their corresponding annotations as the testing set. The rest form a training set of 15,403 images and a validation set of 5,000 images. For each instance, 58 semantic categories are defined and annotated except for the "background" category, i.e. "cap/hat", "helmet", "face", "hair", "left-arm", "right-arm", "left-hand", "right-hand", "protector", "bikini/bra", "jacket/windbreaker/hoodie", "t-shirt", "polo-shirt", "sweater", "singlet", "torso-skin", "pants", "shorts/swim-shorts", "skirt", "stockings", "socks", "left-boot", "right-boot", "left-shoe", "right-shoe", "left-highheel", "right-highheel", "left-sandal", "right-sandal", "left-leg", "right-leg", "left-foot", "right-foot", "coat", "dress", "robe", "jumpsuit", "other-full-body-clothes", "headwear", "backpack", "ball", "bats", "belt", "bottle", "carrybag", "cases", "sunglasses", "eyewear", "glove", "scarf", "umbrella", "wallet/purse", "watch", "wristband", "tie", "other-accessary", "other-upper-body-clothes" and "other-lower-body-clothes". Each instance has a complete set of annotations whenever the corresponding category appears in the current image. Moreover, 2D human poses with 16 dense key points ("right-shoulder", "right-elbow", "right-wrist", "left-shoulder", "left-elbow", "left-wrist", "right-hip", "right-knee", "right-ankle", "left-hip", "left-knee", "left-ankle", "head", "neck", "spine" and "pelvis". Each key point has a flag indicating whether it is visible-0/occluded-1/out-of-image-2) and head & instance bounding boxes are also provided to facilitate Multi-Human Pose Estimation research. 


- Download: The MHP v2.0 dataset is available at [google drive](https://drive.google.com/file/d/1YVBGMru0dlwB8zu1OoErOazZoc8ISSJn/view?usp=sharing) 

- Please refer to our [MHP v2.0 paper](https://arxiv.org/pdf/1804.03287.pdf) (ACM MM'18 [Best Student Paper](http://www.acmmm.org/2018/awards/)) for more details.


### Evaluation Metrics
- Multi-Human Parsing: We use two human-centric metrics for multi-human parsing evaluation, which are initially reported by our [MHP v1.0 paper](https://arxiv.org/pdf/1705.07206.pdf). The two metrics are Average Precision based on part (AP<sup>p</sup>) (%) and Percentage of Correctly parsed semantic Parts (PCP) (%). For evaluation code, please refer to the "Evaluation" folder under our "Multi-Human-Parsing_MHP" repository.


# VisDrone-DroneVehicle

Drone-based RGB-Infrared Cross-Modality Vehicle Detection via Uncertainty-Aware Learning [(paper)](https://arxiv.org/abs/2003.02437).

## Abstract
Drone-based vehicle detection aims at finding the vehicle locations and categories in an aerial image. It empowers smart city traffic management and disaster rescue. Researchers have made mount of efforts in this area and achieved considerable progress. Nevertheless, it is still a challenge when the objects are hard to distinguish, especially in low light conditions. To tackle this problem, we construct a large-scale drone-based RGB-Infrared vehicle detection dataset, termed DroneVehicle. Our DroneVehicle collects 28,439 RGB-Infrared image pairs, covering urban roads, residential areas, parking lots, and other scenarios from day to night. Due to the great gap between RGB and infrared images, cross-modal images provide both effective information and redundant information. To address this dilemma, we further propose an uncertainty-aware cross-modality vehicle detection (UA-CMDet) framework to extract complementary information from cross-modal images, which can significantly improve the detection performance in low light conditions.
An uncertainty-aware module (UAM) is designed to quantify the uncertainty weights of each modality, which is calculated by the cross-modal Intersection over Union (IoU) and the RGB illumination value. Furthermore, we design an illumination-aware cross-modal non-maximum suppression algorithm to better integrate the modal-specific information in the inference phase. Extensive experiments on the DroneVehicle dataset demonstrate the flexibility and effectiveness of the proposed method for cross-modality vehicle detection. 

![VisDrone](https://github.com/VisDrone/DroneVehicle/blob/master/labelsamples.png)

## Dataset
The DroneVehicle dataset consists of a total of 56,878 images collected by the drone, half of which are RGB images, and the resting are infrared images. We have made rich annotations with oriented bounding boxes for the five categories. Among them, car has 389,779 annotations in RGB images, and 428,086 annotations in infrared images, truck has 22,123 annotations in RGB images, and 25,960 annotations in infrared images, bus has 15,333 annotations in RGB images, and 16,590 annotations in infrared images, van has 11,935 annotations in RGB images, and 12,708 annotations in infrared images, and freight car has 13,400 annotations in RGB images, and 17,173 annotations in infrared image. This dataset is available on the download page. 

In DroneVehicle, to annotate the objects at the image boundaries, we set a white border with a width of 100 pixels on the top, bottom, left and right of each image, so that the downloaded image scale is 840 \times 712. When training our detection network, we can perform pre-processing to remove the surrounding white border and change the image scale to 640 \times 512.

### BaiduYun:  
[Train](https://pan.baidu.com/s/1ptZCJ1mKYqFnMnsgqEyoGg) (code:ngar) 

[Validation](https://pan.baidu.com/s/1e6e9mESZecpME4IEdU8t3Q) (code:jnj6)  

[Test](https://pan.baidu.com/s/1JlXO4jEUQgkR1Vco1hfKhg) (code:tqwc) 

### GoogleDrive:   
googledrive link will be released soon.

![VisDrone](https://github.com/VisDrone/DroneVehicle/blob/master/dataset_sample.png)

### Code:
[UA-CMDet](https://github.com/SunYM2020/UA-CMDet)

## Citation 

Please cite this paper if you want to use it in your work.
```
@ARTICLE{sun2020drone,
  title={Drone-based RGB-Infrared Cross-Modality Vehicle Detection via Uncertainty-Aware Learning}, 
  author={Sun, Yiming and Cao, Bing and Zhu, Pengfei and Hu, Qinghua},
  journal={IEEE Transactions on Circuits and Systems for Video Technology}, 
  year={2022},
  volume={},
  number={},
  pages={1-1},
  doi={10.1109/TCSVT.2022.3168279}
}
```




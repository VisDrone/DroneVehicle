# VisDrone-DroneVehicle

![VisDrone](https://github.com/VisDrone/DroneVehicle/blob/master/dataset_sample.png)

# Abstract
Drone-based vehicle detection aims at finding the vehicle locations and categories in an aerial image. It empowers smart city traffic management and disaster rescue. Researchers have made mount of efforts in this area and achieved considerable progress. Nevertheless, it is still a challenge when the objects are hard to distinguish, especially in low light conditions. To tackle this problem, we construct a large-scale drone-based RGB-Infrared vehicle detection dataset, termed DroneVehicle. Our DroneVehicle collects 28,439 RGB-Infrared image pairs, covering urban roads, residential areas, parking lots, and other scenarios from day to night. Due to the great gap between RGB and infrared images, cross-modal images provide both effective information and redundant information. To address this dilemma, we further propose an uncertainty-aware cross-modality vehicle detection (UA-CMDet) framework to extract complementary information from cross-modal images, which can significantly improve the detection performance in low light conditions.
An uncertainty-aware module (UAM) is designed to quantify the uncertainty weights of each modality, which is calculated by the cross-modal Intersection over Union (IoU) and the RGB illumination value. Furthermore, we design an illumination-aware cross-modal non-maximum suppression algorithm to better integrate the modal-specific information in the inference phase. Extensive experiments on the DroneVehicle dataset demonstrate the flexibility and effectiveness of the proposed method for cross-modality vehicle detection. 

![VisDrone](https://github.com/VisDrone/DroneVehicle/blob/master/label_sample.png)

## Dataset
The DroneVehicle dataset consists of a total of 56,878 images collected by the drone, half of which are RGB images, and the resting are infrared images. We have made rich annotations with oriented bounding boxes for the five categories. Among them, car has $389,779$ annotations in RGB images, and $428,086$ annotations in infrared images, \textit{truck} has $22,123$ annotations in RGB images, and $25,960$ annotations in infrared images, \textit{bus} has $15,333$ annotations in RGB images, and $16,590$ annotations in infrared images, \textit{van} has $11,935$ annotations in RGB images, and $12,708$ annotations in infrared images, and \textit{freight car} has $13,400$ annotations in RGB images, and $17,173$ annotations in infrared image.

## Citation 

Please cite this paper if you want to use it in your work.
```
@misc{zhu2020drone,
    title={Drone-based RGB-Infrared Cross-Modality Vehicle Detection via Uncertainty-Aware Learning},
    author={Yiming Sun and Bing Cao and Pengfei Zhu and Bin Xiao and Qinghua Hu},
    year={2021},
    eprint={},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}
```




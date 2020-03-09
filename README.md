# VisDrone-DroneVehicle

![VisDrone](https://github.com/VisDrone/DroneVehicle/blob/master/dataset_sample.png)

Camera-equipped drones can capture targets on the ground from a wider field of view than static cameras or moving
sensors over the ground. In this project, we present a large-scale vehicle detection and counting benchmark, named DroneVehicle,
aiming at advancing visual analysis tasks on the drone platform. The images in the benchmark were captured over various urban
areas, which include different types of urban roads, residential areas, parking lots, highways, etc., from day to night. Specifically,
DroneVehicle consists of 15,532 pairs of images, i.e., RGB images and infrared images with rich annotations, including oriented object bounding boxes, object categories, etc. With intensive amount of effort, our benchmark has 441,642 annotated
instances in 31,064 images.

The challenge mainly focuses on two tasks: 

Task 1: object detection in images. Given a predefined
set of object classes (e:g:, car, bus, and truck), the task
aims to detect objects of these classes from individual
images taken from drones.

Task 2: object counting in images. The task aims to
estimate the number of vehicles from individual images
in DroneVehicle

![VisDrone](https://github.com/VisDrone/DroneVehicle/blob/master/label_sample.png)

## Citation 

@misc{zhu2020drone,
    title={Drone Based RGBT Vehicle Detection and Counting: A Challenge},
    author={Pengfei Zhu and Yiming Sun and Longyin Wen and Yu Feng and Qinghua Hu},
    year={2020},
    eprint={2003.02437},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}



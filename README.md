# TVD Dataset: A Benchmark for Object Detection

Welcome to the TVD Dataset – a comprehensive benchmark for object detection tasks!

### Introduction
The TVD Dataset offers a rich collection of images spanning 7 classes of vehicles, including cars, motorcycles, buses, trucks, vans, and notably, ambulances and fire trucks. Designed specifically to aid in the identification of traffic patterns, this dataset is tailored for processing video images using deep neural networks, with a special focus on facilitating the movement of emergency vehicles.

### Dataset Overview
- **Total Images**: 29,759
- **Training Images**: 25,369
- **Validation Images**: 2,896
- **Test Images**: 1,494

### Dataset Samples
Below is a glimpse of the dataset with an example of its images:

<p align="center">
    <img src="https://user-images.githubusercontent.com/61584820/205639613-1467347c-da59-4c76-870b-3f0cdf1f731d.png" width="70%" height="70%">
</p>
---
Feel free to explore the dataset further and leverage it for your object detection tasks!

------------------------------------------------------------------

## Download Dataset

You can use the Google Drive link below to download the dataset. Before downloading, please make sure to read the license data provided in this section.

| Method | Address |
| ------ | ------- |
| Download from Google Drive ➡️ | [Google Drive Link](https://drive.google.com/file/d/1h-McuzhBSoeTRcovNotVUXCSp__jgTaH/view?usp=sharing) |

---

To understand the accuracy of this project for video, you can watch the video below:

<!-- Insert your video link here -->


------------------------------------------------------------------
## Dataset Preparation

The TVD dataset images are randomly divided into three parts: training data, validation data, and test data. The test images are completely separate from the training dataset, offering one of the advantages of this dataset.

```bash
TVD dataset
├── Train Dataset
│   ├── Ambulance ----> 484 images
│   ├── Bus-----------> 5000 images
│   ├── Car-----------> 5000 images
│   ├── Motorcycle----> 5000 images
│   ├── Truck---------> 4658 images
│   ├── Van-----------> 4727 images
│   └── Firetruck-----> 500 images
├── Validation Dataset
│   ├── Ambulance ----> 65 images
│   ├── Bus-----------> 638 images
│   ├── Car-----------> 638 images
│   ├── Motorcycle----> 587 images
│   ├── Truck---------> 473 images
│   ├── Van-----------> 405 images
│   └── Firetruck-----> 90 images
└── Test Dataset
    ├── Ambulance ----> 7 images
    ├── Bus-----------> 256 images 
    ├── Car-----------> 501 images
    ├── Motorcycle----> 176 images
    ├── Truck---------> 385 images
    ├── Van-----------> 150 images
    └── Firetruck-----> 19 images


--------------------------------------------------------------------
## Train YOLO

Algorithms for detecting objects of YOLO versions 5, 6, and 7 have been trained with the help of this dataset. Finally, the best results are related to YOLO version 7, which has reached a final Precision of 85%, mAP_0.5 of 85%, and mAP_0.5:0.9 of 64%.

The results obtained for different versions are summarized in the table below:

| YOLO Version | Number of Epochs | Average Precision (AP) IoU=0.5 | Average Precision (AP) IoU=0.5:0.95 | Recall |
| ------------ | ---------------- | ------------------------------ | ----------------------------------- | ------ |
| YOLOv5s      | 100 epochs        | 81.90%                         | 60.70%                              | 70.50% |
| YOLOv6-s     | 30 epochs         | 81%                            | 60.40%                              | 73.80% |
| YOLOv7       | 55 epochs         | 85%                            | 64.70%                              | 76%    |

The table below shows more detailed results of the output of version 7 of the YOLO algorithm on the validation data trained by the proposed dataset:

| Class Name  | Precision | Recall | mAP 50% | mAP 50% - 90% |
| ----------- | --------- | ------ | -------- | -------------- |
| All classes | 85%       | 76%    | 85%      | 64%            |
| Ambulance   | 81.30%    | 75.30% | 81.20%   | 69.90%         |
| Bus         | 91.30%    | 83.90% | 90.80%   | 76.10%         |
| Car         | 86.60%    | 58%    | 77.90%   | 53.10%         |
| Motorcycle  | 90.10%    | 79.80% | 87.90%   | 56.40%         |
| Truck       | 82.30%    | 76%    | 85.40%   | 62.50%         |
| Van         | 79.10%    | 88.20% | 91%      | 79.70%         |
| FireTruck   | 85.20%    | 70.50% | 80.80%   | 55%            |

---

## Train again or test dataset

If you want to train this dataset again or try the results for another category of images or videos, you can use the final weight file by using the Google Drive link to download the best weight YOLOv7 after training with the TVD dataset.

| 🙂 | Address |
| - | ------- |
| Download best weight from Google Drive ➡️ | [Best Weight](https://drive.google.com/file/d/1SdFQogWndCprFZ5SivoSKVyzooNw0Tel/view?usp=sharing) |

Or use the [TVD_dataset_yolov7.ipynb](/TVD_dataset_yolov7.ipynb/) for more guidance and train again or test weight with new pictures.

------------------------------------------------------------------
# License

# License

1. This dataset (TVD dataset) is made available for academic use only.
2. If you use this dataset in your research, you should refer to the GitHub repository and the address of the article
 published on this topic at
| [Object Detection for Vehicles with Yolo](https://ieeexplore.ieee.org/abstract/document/10432884) |




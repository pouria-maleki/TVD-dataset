# TVD-dataset
A new Benchmark for object detection 

### dataset of 7 classes of vehicles including car, motorcycle, bus, truck, van and especially ambulance and firetruck are presented which can be used to identify traffic by processing video images with the help of deep neural networks with emphasis on facilitating the movement of emergency vehicles. The images of this dataset have been obtained from free internet sources, which are a total of 29759 images, of which 25369 are train images, 2896 are validation images, and 1494 are test images. 

An example of dataset images can be seen in the figure below .
<p align="center">
        <img src="https://user-images.githubusercontent.com/61584820/205639613-1467347c-da59-4c76-870b-3f0cdf1f731d.png" width=70% height=70%>
</p>

------------------------------------------------------------------

## download Dataset
You can use the Google Drive link below to download the dataset.
Warning: Be sure to read the license data in this section before downloading it 

 | method | addres |
| - | - |
| Download from google drive ---> <br>  |[google drive link ](https://drive.google.com/file/d/1h-McuzhBSoeTRcovNotVUXCSp__jgTaH/view?usp=sharing)



 To understand the accuracy of this project for video you can watch the video below : 

 To train our detector we take the following steps:

------------------------------------------------------------------
## Dataset preparation 
Dataset images are randomly divided into three parts: training data, validation data, and test data .
The test images are completely outside the training dataset, and this is one of the advantages of this dataset.


```bash
TVD dataset
├──Train Dataset
│   ├── Ambulance ---->484  images
│   ├── Bus----------->5000 images
│   ├── Car----------->5000 images
│   ├── Motorcycle---->5000 images
│   ├── Truck--------->4658 images
│   ├── Van----------->4727 images
│   └── Firetruck----->500  images
├── Validation Dataset
│   ├── Ambulance ---->65   images
│   ├── Bus----------->638  images
│   ├── Car----------->638  images
│   ├── Motorcycle---->587  images
│   ├── Truck--------->473  images
│   ├── Van----------->405  images
│   └── Firetruck----->90   images
├── Test Dataset
│   ├── Ambulance ---->7   images
│   ├── Bus----------->256 images 
│   ├── Car----------->501 images
│   ├── Motorcycle---->176 images
│   ├── Truck--------->385 images
│   ├── Van----------->150 images
│   └── Firetruck----->19  images

```
The number of objects per split, the average number of objects per image, and the number of classes for our Dataset (TVD dataset) can be seen in the figure below.
<p align="center">
        <img src="[+](https://user-images.githubusercontent.com/61584820/205649170-36540307-d8c7-4d29-91d3-ad944bb72f45.png)" width=70% height=70%>
</p>

--------------------------------------------------------------------
## Train yolo 
Algorithms for detecting objects of Yolo version 5, 6 and 7 have been trained with the help of this dataset. Finally, the best results are related to Yolo version 7, which has reached 85% final Precision and mAP_0.5 to 85% and mAP_0.5:0.9 to 64%.
The results obtained for different versions are summarized in Table below.
### Training the network for all versions continued until the data validation error is reduced and the process of increasing the precision of the network has been fixed. 

| Yolo version | The number of epoch | Average Precision  (AP)  IoU=0/50 | Average Precision  (AP) IoU=0/50:0/95 | recall |
| --- | --- | --- | --- | --- |
|YOLOV5s |100 epoch |81/90% |60/70% |70/50% |
| YOLOV6-s | 30 epoch |81% |60/40% |73/80% |
| YOLOV7 | 55 epoch |85% |64/70% |76% |


Table below shows the more detailed results of the output of  version 7 of the YOLO algorithm on the validation data trained by the proposed dataset
| class Name | percision | Recal | mAP 50% | mAP 50% - 90% |
| --- | --- | --- | --- | --- |
|all class |85% |76% |85% |64% |
|Ambulance |81/30% |75/30% |81/20% |69/90% |
|Bus |91/30% |83/90% |90/80% |76/10% |
|Car |86/60% |58% |77/90% |53/10% |
|Motorcycle |90/10% |79/80% |87/90% |56/40% |
|Truck |82/30% |76% |85/40% |62/50% |
|Van |79/10% |88/20% |91% |79/70% |
|FireTruck |85/20% |70/50% |80/80% |55% |


------------------------------------------------------------------
## Train again or test dataset
If you want to train this dataset again or try the results for another category of images or videos, you can use the final weight file by use the Google Drive link to download the best weight yolov7 after train with TVD dataset.
 | :) | addres |
| - | - |
| Download best weight from google drive ---> <br>  |[best weight ](https://drive.google.com/file/d/1SdFQogWndCprFZ5SivoSKVyzooNw0Tel/view?usp=sharing)


or use the  [TVD_dataset_yolov7.ipynb](/TVD_dataset_yolov7.ipynb/)  for more guidance and train again or test weight with new pictures .

------------------------------------------------------------------
# license
If you use this dataset in your research or work, you should tag this GitHub and our article that will be published soon.

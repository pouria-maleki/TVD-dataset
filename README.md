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
Warning: Be sure to read the license data in this section before downloading it.1- Download from Roboflow :

 | method | addres |
| - | - |
| Download from google drive ---> <br>  |[google drive link ](https://badaninjamizanam!)



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
###Training the network for all versions continued until the data validation error is reduced and the process of increasing the precision of the network has been fixed. 

| Command | Description | Command | Description | Description |
| --- | --- | --- | --- | --- |
|asas |asas |asas |asass |asas |
| git diff | sd |sdsd |sdsd |sdsd |sdsds |





Table 5 shows the more detailed results of the output of this version of the YOLO algorithm on the validation data trained by the proposed dataset

<p align="center">
        <img src="https://user-images.githubusercontent.com/61584820/185476694-feae43d0-9696-4543-bd7c-e8354c0725af.png" width=70% height=70%>
</p>


![results](https://user-images.githubusercontent.com/61584820/185478214-c68b534c-93be-41fe-8d5f-51da82b0bb89.png)

------------------------------------------------------------------
## Train again or test dataset
If you want to train this dataset again or try the results for another category of images or videos, you can use the final weight file [best.pt](/best.pt/) or use the  [iranian_vehicle_dataset_Train_Yolov5.ipynb](/iranian_vehicle_dataset_Train_Yolov5.ipynb/)  for more guidance.

iranian_vehicle_dataset_Train_Yolov5.ipynb
# license
If you use this dataset in your research or work, you should tag this GitHub and our article that will be published soon.

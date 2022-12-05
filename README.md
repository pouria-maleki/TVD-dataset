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
│   ├── CAr----------->5000 images
│   ├── Motorcycle---->5000 images
│   ├── Truck--------->4658 images
│   ├── Van----------->4727 images
│   └── Firetruck----->500  images
├── Validation Dataset
│   ├── Ambulance ---->65   images
│   ├── Bus----------->638  images
│   ├── CAr----------->638  images
│   ├── Motorcycle---->587  images
│   ├── Truck--------->473  images
│   ├── Van----------->405  images
│   └── Firetruck----->90   images
├── Test Dataset
│   ├── Ambulance ---->7   images
│   ├── Bus----------->256 images 
│   ├── CAr----------->501 images
│   ├── Motorcycle---->176 images
│   ├── Truck--------->385 images
│   ├── Van----------->150 images
│   └── Firetruck----->19  images

```

3 directories, 7 files
<p align="center">
        <img src="https://user-images.githubusercontent.com/61584820/181755020-5157db78-fe2c-469a-882e-82b63df3aa7b.png" width=70% height=70%>
</p>



| :) | class name |  number of annotation  |
| - | - | - |
| 1 | car <br>  |4333   
| 2 | bus <br>  |893
| 2 | Truck <br>  |539
------------------------------------------------------------------
## Train again or test dataset
If you want to train this dataset again or try the results for another category of images or videos, you can use the final weight file [best.pt](/best.pt/) or use the  [iranian_vehicle_dataset_Train_Yolov5.ipynb](/iranian_vehicle_dataset_Train_Yolov5.ipynb/)  for more guidance.

iranian_vehicle_dataset_Train_Yolov5.ipynb
--------------------------------------------------------------------
## results 
The overall accuracy of the network is 93% and the overall mAP of the network for the threshold limit of 50% is equal to 92.7% .Other results and criteria are given in the following table and figure.

<p align="center">
        <img src="https://user-images.githubusercontent.com/61584820/185476694-feae43d0-9696-4543-bd7c-e8354c0725af.png" width=70% height=70%>
</p>


![results](https://user-images.githubusercontent.com/61584820/185478214-c68b534c-93be-41fe-8d5f-51da82b0bb89.png)


# license
If you use this dataset in your research or work, you should tag this GitHub and our article that will be published soon.

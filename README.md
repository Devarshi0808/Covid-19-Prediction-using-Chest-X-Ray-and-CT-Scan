# COVID-19-Detection-using-on-Chest-X-rays-and-CT-Scans
COVID-19 Detection based on Chest X-rays and CT Scans using four Transfer Learning algorithms: VGG16, ResNet50, InceptionV3, Xception. The models were trained for 500 epochs on around 1000 Chest X-rays and around 750 CT Scan images on Google Colab GPU. After training, the accuracies acheived for the model are as follows:


                InceptionV3  VGG16   ResNet50   Xception
Chest X-rays    96%          94%      83%       92%

CT Scans        93%          93%      80%       95%


A Flask App was later developed wherein user can upload Chest X-rays or CT Scans and get the output of possibility of COVID infection.


# Dataset
The dataset for the project was gathered from two sources:
1. Chest X-ray images (1000 images) were obtained 
2. CT Scan images (750 images) were obtained 
80% of the images were used for training the models and the remaining 20% for testing

# Evaluation and Results
Sample output of test images.....
  Images in screenshots folder

 Make sure you follow these steps otherwise Flask App will not work properly. Also make sure you have PYTHON V 3.6.9. Other versions might not be supported

To download python file use the link https://drive.google.com/file/d/1KOn9hB-a2S6ZEVdLuOIdiKSuUBUd2p51/view?usp=sharing
                                                  OR
To download software for pycharm community use the link  https://www.jetbrains.com/pycharm/

use this viedo to create a environment https://youtu.be/W8C097f6Hcg

Screenshots of Flask App

For more screenshots, please visit the screenshots folder

# Technical Concepts
1. ImageNet is formally a project aimed at (manually) labeling and categorizing images into almost 22,000 separate object categories for the purpose of computer vision research.

2. ResNet50 ResNet-50 is a convolutional neural network that is 50 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. Unlike traditional sequential network architectures such as AlexNet, OverFeat, and VGG, ResNet is instead a form of “exotic architecture” that relies on micro-architecture modules.

3.VGG16 is a convolutional neural network model proposed by K. Simonyan and A. Zisserman from the University of Oxford in the paper “Very Deep Convolutional Networks for Large-Scale Image Recognition”. The model achieves 92.7% top-5 test accuracy in ImageNet, which is a dataset of over 14 million images belonging to 1000 classes.

4. Inception-V3 is a convolutional neural network that is 48 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. As a result, the network has learned rich feature representations for a wide range of images. The network has an image input size of 299-by-299.

5. Xception is a convolutional neural network that is 71 layers deep. You can load a pretrained version of the network trained on more than a million images from the ImageNet database. The pretrained network can classify images into 1000 object categories, such as keyboard, mouse, pencil, and many animals. As a result, the network has learned rich feature representations for a wide range of images. The network has an image input size of 299-by-299.


## How to use Flask App

        
     pip install -r requirements.txt
 
  On command prompt, run 
            
python app.py

  Open your web browser and go to  127.0.0.1:5000   to access the Flask App 






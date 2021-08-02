# MEng-Diploma-Thesis
Diploma Thesis: "Transfer learning from supervised and unsupervised pre-trained convolutional neural networks for the recognition of skin lesions"

Supervisor: Aristidis Likas


## Introduction

In the diploma thesis, two methods belonging to the category of self-supervised contrastive learning (MoCo and SimCLR) are studied and compared with the classic method of supervised training of convolutional neural networks. In addition, the selection of the best intermediate convo- lutional layer for the extraction of representations in order to use it in the transfer learning for the training of another neural network is also studied.The pre-trained convolutional neural network ResNet-50 was used for this study, which has been trained differerently depending on the method. The purpose of the network is the automatic recognition of skin lesions in clinical images and more specifically the recognition of Actinic Keratosis (AK) from healthy skin and Seborrheic Keratosis (SK). We concluded that the classic training of the convolutional neural network has better results on this particular problem, while the second intermediate convolutional layer is the best, as in texture separation, the first convolutional layers are the most satisfactory.


## Dataset

Our dataset consist of images from 23 patients from university hospital of Ioannina. Dermatologists depict to us the regions that are interest (ROI). Those images, that used for training and evaluating our model, have shape 50x50. In total we had 4629 ROI images of Actinic Keratosis, 7002 ROI images of Healthy Skin and 945 ROI images of Seborrheic Keratosis.

For reasons of personal data security, I can not upload the images used in this diploma thesis.


## Results
We studied and compared the performance of 2 self-supervised contrastive learning methods, SimCLR and MoCo, with the classical method of training convolutional neural networks, as well as the selection of the best intermediate convolutional layer for the extraction of representations in order to use it in the transfer learning for the training of another neural network. The pre-trained convolutional neural network ResNet-50 was used for this study. The purpose of the network is the automatic recognition of skin lesions in clinical images and more specifically the recognition of Actinic Keratosis (AK) from healthy skin and Seborrheic Keratosis (SK). 23 different trainings of the network were done on different training and control sets (23 different patients) in order to reach safe conclusions. We concluded that the classical method of training the convolutional neural network has better results, while at the same time we have shown that the best intermediate convolutional layer of ResNet-50, for extracting representations for training a neural network, is layer 2. Thus in texture separation the first convolutional intermediate layers are more satisfactory.

Examples

![image01](https://user-images.githubusercontent.com/25775552/127875958-444c64b6-9371-452e-829d-e84422f72b98.png)

----------------------------------------------------------------------------

![image02](https://user-images.githubusercontent.com/25775552/127876148-0f2c85ee-d77f-4a85-9002-6dba7c487225.png)

Some information about the images:

1) the outline with the dark blue is the area that the doctor has determined to be the AK. The doctors locate an area but they do not find the cancerous outline in great detail

2) The outline in light blue, is the area that our model has recognized to be AK, and indeed it is (True Positive).

3) The outline in black, is the area that our model has recognized as AK, while it is not (False Positive)

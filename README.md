# MEng-Diploma-Thesis
Diploma Thesis: "Transfer learning from supervised and unsupervised pre-trained convolutional neural networks for the recognition of skin lesions"

Supervisor: Aristidis Likas


Introduction

In the diploma thesis, two methods belonging to the category of self-supervised contrastive learning (MoCo and SimCLR) are studied and compared with the classic method of supervised training of convolutional neural networks. In addition, the selection of the best intermediate convo- lutional layer for the extraction of representations in order to use it in the transfer learning for the training of another neural network is also studied.The pre-trained convolutional neural network ResNet-50 was used for this study, which has been trained differerently depending on the method. The purpose of the network is the automatic recognition of skin lesions in clinical images and more specifically the recognition of Actinic Keratosis (AK) from healthy skin and Seborrheic Keratosis (SK). We concluded that the classic training of the convolutional neural network has better results on this particular problem, while the second intermediate convolutional layer is the best, as in texture separation, the first convolutional layers are the most satisfactory.


Dataset

Our dataset consist of images from 23 patients from university hospital of Ioannina. Dermatologists depict to us the regions that are interest (ROI). Those images, that used for training and evaluating our model, have shape 50x50. In total we had 4629 ROI images of Actinic Keratosis, 7002 ROI images of Healthy Skin and 945 ROI images of Seborrheic Keratosis.

For reasons of personal data security, I can not upload the images used in this diploma thesis.

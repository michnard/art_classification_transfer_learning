# Artist classification
## Given the painting, decide who drew it.

### Data
The data is based on the dataset available on Kaggle at https://www.kaggle.com/ikarus777/best-artworks-of-all-time by Icaro (Ikarus777), under CC BY-NC-SA 4.0.

I selected 9 artists out of the total 50 available, took 100 images (for each artist) as training dataset (i.e. 900 images in total) and 20~50 images per artist, depending on availability (total ~380) as test data.

The artists are:
['Albrecht_Durer', 'Amedeo_Modigliani', 'Frida_Kahlo', 'Gustav_Klimt', 'Leonardo_da_Vinci', 'Pablo_Picasso', 'Sandro_Botticelli', 'Titian', 'Vincent_van_Gogh']

The data used for this specific notebook can be found here:
train data: https://drive.google.com/drive/folders/1o2BicG7gCHC29w8ulTTUCix3XMb9BmZx?usp=sharing
test data: https://drive.google.com/drive/folders/1zwoV84ksMIfPytDvmxGbHBnk4M8iYY0B?usp=sharing

### Method
I'm gonna use different deep learning architechtures, pretrained on ImageNet (as avalable from pytorch: https://pytorch.org/vision/stable/models.html) and train only the output layer.

Transfer learning acknowledgements: this exercise was inspired by the project of Jama Hussein Mohamud & Alex Hernandez-Garcia during Neuromatch Academy 2021 (https://deeplearning.neuromatch.io/projects/ComputerVision/transfer_learning.html). Part of the code is also (loosely) based on Sasank Chilamkurthy's "TRANSFER LEARNING FOR COMPUTER VISION TUTORIAL" (https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html).

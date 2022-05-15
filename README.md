# Mood-Classifier

Classifies your Mood/Emotion based on your facial expressions with fastai deep learning library

## Dataset:

https://www.kaggle.com/datasets/jonathanoheix/face-expression-recognition-dataset  
*Dataset is quite noisy with alot of mislabelled data.*

## Details:

* Pretrained models used for comparison: resnet34, resnet50, resnet101 | vgg16_bn, vgg19_bn,
*finalized on resnet50 and vgg19_bn*

* Optimal LR was determined several times.
* Data cleaning was done through ImageClassifierCleaner GUI but still detailed cleaning is needed.

* Through multiple model testings, none of the models seem to cross 70% accuracy.
Accuracy is not a priority in this project, though overfitting is seen.
Actual efficiency has to be seen through deployment.

  *May build a model from scratch to eliminate the possibility of the dataset not generalizing to the pretrained model.*

* Planned deployment through AWS Lambda.

## To test real time predictions:

1. Copy / Star the 'Mood.pkl' file to your drive:   
 https://drive.google.com/file/d/1jmiEUuDjbTBN10sYx5gyJ3bjGI1yArQW/view?usp=sharing

2. Open this Colab Notebook, mount your drive and copy the 'Mood.pkl' file path to the cell indicated and execute: https://colab.research.google.com/drive/1NmOAVLm51kfznmkKz7bn4la3bRrM93z7?usp=sharing

   To have a closer look check out this file: [Test_Prediction(realtime).ipynb](Test_Prediction(realtime).ipynb)

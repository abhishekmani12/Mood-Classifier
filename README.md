# Mood-Classifier

Classifies your Mood/Emotion based on your facial expressions with fastai deep learning library

Dataset:
https://www.kaggle.com/datasets/jonathanoheix/face-expression-recognition-dataset

Dataset is quite noisy with alot of mislabelled data.

Pretrained models used for comparison: resnet34, resnet50, resnet101 | vgg16_bn, vgg19_bn

Finalized on resnet50

Optimal LR was determined several times.

Data cleaning was done through ImageClassifierCleaner GUI but still detailed cleaning is needed.

Through multiple model testings, none of the models seem to cross 70% accuracy.
Accuracy is not a priority in this project, though overfitting is seen.


Actual efficiency has to be seen through deployment.

May build a model from scratch to eliminate the possibility of the dataset not generalizing to the pretrained model.

Planned deployment through AWS Lambda.

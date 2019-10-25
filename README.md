# Robotic-grasping-cornell

In this project, Deep Convolutional Neural Networks (DCNNs) is used to simultanously detect a grasping point and angle of an object, so that a robot arm can pick the object. In general, this is the implementation of a small model of the model presented in this paper https://arxiv.org/abs/1802.00520. We do not implement the Grasp Proposal Networks, so instead of using 2-stage DCNNs, we use one-stage DCNNs.

## Support
+ python 3.6.8
+ pytorch 1.0.0

## Codes
1. Data preprocessing
2. Training
3. Demo

### 1. Data preprocessing
Plese follow this repo: https://github.com/ivalab/grasp_multiObject_multiGrasp

1.1) Download [Cornell Dataset](http://pr.cs.cornell.edu/grasping/rect_data/data.php) 

1.2) Run `dataPreprocessingTest_fasterrcnn_split.m` (please modify paths according to your structure)  

### 2. Training
'''
$ python3 train.py --epochs 100 --lr 0.0001 --batch_size 8
'''

### 3. Demo
+ Download the pretrained model [dropbox drive](https://drive.google.com/drive/folders/1Tf0nepgfYp3L8Vm6nppsURm5x9S_qBB) 
+ Put in the folder `./models`
+ Run demo:
'''
$ python3 demo.py
'''

### Acknowledgment

This repo borrows some of code from
https://github.com/ivalab/grasp_multiObject_multiGrasp




# NSynth
This repository contains material related to Udacity's Machine Learning Engineer Nando Degree (MLEND) capstone project. The objective of this project is to classify wave files (.wav) based on their instrument family. 

The findings of can be found in Report.pdf. The report is also available in this link:
https://drive.google.com/file/d/1sgq-3WGUuPyAjt-HeDCNTQkCAE9ZZ7vc/view?usp=sharing

The instrument classification using the NSynth dataset found here:
https://magenta.tensorflow.org/datasets/nsynth

Due to the size of the dataset it can't be stored on a repository.
The sampled training files are 60MB+ in size and can't be stored in this repo.

All scripts are written in python, and it is assumed that the user already has Anaconda or another python interpreter installed.
If not, please download Anaconda from the link below:
https://docs.anaconda.com/anaconda/install/

The required libraries for this repository are:
- numpy
- pandas
- matplotlib.pyplot
- librosa
- os
- glob
- re
- scipy
- time
- collections
- scipy
- keras
- pickle
- itertools
- sklearn

The above packages are most likely built in your Anaconda package with the exception of Librosa which needs to be installed.

The time required to run most scripts depends on the user's machine. For example, extracing spectral features from 50,000 files requires more than 3hours on a 2014 Macbook Pro.

For the convolutional neural network (CNN), it is recommended to use Amazon Web Services (AWS) or an equivalent cloud computing service. For this project the EC2 instance is p2.xlarge using <i>"Deep Learning AMI with Source Code -CUDA 8- Ubuntu"</i>.


## Looking Ahead
I passed and obtained my degree, looking forward to more exciting projects!

![MLEND_NK](https://drive.google.com/file/d/1kXYhXxQH0nIrPjXuhR-7CNu51Zas5hpJ/view?usp=sharing)

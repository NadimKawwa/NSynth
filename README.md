# NSynth
This repository contains material related to Udacity's Machine Learning Engineer Nando Degree (MLEND) capstone project. The objective of this project is to classify wave files (.wav) based on their instrument family. 

Like many people, I listen to music on a daily basis. I'm also fascinated how streaming giants such as Apple, Spotify,  Tidal, and Pandora (just to name a few) can curate songs and recommend them to users. The first step to recommending

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


## Summary of Results
The ultimate winner in terms of accuracy and effciency was Random Forests, at 65% efficiency. The second runner up was CNN at 56% accuracy. The plot below shows the confusion matrix for the model.

![RF_confusion_matrix](https://github.com/NadimKawwa/NSynth/blob/master/ConfusionMatrix/RF_Normalized_RandomSearch.png)



Because we used a subset of the data for training, the next logical step was a sensitivy test to see how wildy how results would vary if we had used another set. Unsurprisingly, using a whole net training set gave us 85% accuracy. This raises the question: could another subset of the data returned a worse performance?

It's important to keep in mind that the paramters we initialize will affect our results. The key factor for predicting success in any machine learning exercise is the data.


## Looking Ahead
I passed and obtained my degree, looking forward to more exciting projects!

![MLEND_NK](https://github.com/NadimKawwa/NSynth/blob/master/MLEND.png)


## Acknowledgments 

The findings presented here could not have been possible without the generosity of researchers who made their findings public.

[1] Jesse Engel, Cinjon Resnick, Adam Roberts, Sander Dieleman, Douglas Eck, Karen Simonyan, and Mohammad Norouzi. "Neural Audio Synthesis of Musical Notes with WaveNet Autoencoders." 2017.
[2] Learning Multiple Layers of Features from Tiny Images, Alex Krizhevsky, 2009.
[3] Introduction to machine learning with Python: a guide for data scientists
Andreas Müller-Sarah Guido - O'Reilly. - 2017
[4] https://hypertextbook.com/facts/2003/ChrisDAmbrose.shtml
[5] http://www.electropedia.org/iev/iev.nsf/display?openform&ievref=801-30-04
[6] https://ccrma.stanford.edu/CCRMA/Courses/152/percussion.html
[7] Fitzgerald, Derry. “Harmonic/percussive separation using median filtering.” 13th International Conference on Digital Audio Effects (DAFX10), Graz, Austria, 2010.
[8] Meinard Müller and Sebastian Ewert “Chroma Toolbox: MATLAB implementations for extracting variants of chroma-based audio features” In Proceedings of the International Conference on Music Information Retrieval (ISMIR), 2011.
[9] https://ccrma.stanford.edu/~jos/st/Spectrograms.html
[10] Roger B. Dannenberg, Introduction to Computer Music Spectral Centroid
[11] Jiang, Dan-Ning, Lie Lu, Hong-Jiang Zhang, Jian-Hua Tao, and Lian-Hong Cai. “Music type classification by spectral contrast feature.” In Multimedia and Expo, 2002. ICME‘02. Proceedings. 2002 IEEE International Conference on, vol. 1, pp. 113-116. IEEE, 2002.
[12] arXiv:1412.6980 [cs.LG]


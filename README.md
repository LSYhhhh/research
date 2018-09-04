
Brain Signal Anaylsis Projects
==========

This repository contains groups of scripts written as a part of EEG classification research for 
the state-of-the-art deep learning application. Collaborated with researchers at Columbia University Medical Center.

Overview
--------

TensorFlow API, Keras implementation of Zhang et al(2018), "EEG-based Intention Recognition from Spatio-Temporal Representations via Cascade and Parallel Convolutional Recurrent Neural Networks" for EEG motar imagery classification on PhysioNet data (https://www.physionet.org/pn4/eegmmidb/). Stacked CNN and RNN were applied on time-distributed sliding windows of raw EEG data.


Acamdemic Papers
------------

directory | title                                               |  author                             |        year
--------|-------------------------------------------------------|-------------------------------------|-----------------
BCI4 | Filter Bank Common Spatial Pattern (FBCSP) in Brain-Computer Interface | Kai Keng Ang, et al.                 | 2008
BCI4 | Filter bank common spatial pattern algorithm on BCI competition IV Datasets 2a and 2b | Kai Keng Ang, et al.               | 2012
BCI4 | Feature Selection for Motor Imagery EEG Classification Based on Firefly Algorithm and Learning Automata    | Aiming Liu, et al. | 2017
deepLearning  | Learning Representations from EEG with Deep Recurrent-Convolutional Neural Networks          | Pouya Bashivan, et al. | 2016
deepLearning  | EEG-Based Emotion Recognition Using Deep Learning Network with Principal Component Based Covariate Shift Adaptation | Suwicha Jirayucharoensak, et al.                        | 2014
deepLearning  | A Deep Learning Architecture for Temporal Sleep Stage Classification Using Multivariate and Multimodal Time Series | Stanislas Chambon, et al.                        | 2018
deepLearning  | Deep Learning With Convolutional Neural Networks for EEG Decoding and Visualization |Robin T. Schirrmeister, et al.   | 2017
deepLearning     | EEG-based Intention Recognition from Spatio-Temporal Representations via Cascade and Parallel Convolutional Recurrent Neural Networks | Dalin Zhang, et al. | 2018
deepLearning | A Deep Learning Method for Classification of EEG Data Based on Motor Imagery                | Xiu An, et al.               | 2014
emotionState | Classifying Different Emotional States by Means of EEG- Based Functional Connectivity Patterns              | You-Yun Lee, Shulan Hsieh                | 2014
emotionState | Emotion Classification Based on Gamma-band EEG
              | Mu Li, Bao-Liang Lu                | 2009
preprocessing | Time-series discrimination using feature relevance analysis in motor imagery classification              | A.M. Alvarez-Meza, et al.                | 2014
preprocessing | Comparison of signal decomposition methods in classification of EEG signals for motor-imagery BCI system              | Jasmin Kevric, et al.                | 2015
preprocessing | Classification of EEG Motor imagery multi class signals based on Cross Correlation | D.Hari Krishna, et al.                | 2016
preprocessing | EEG Signal Processing Techniques For Mental Task Classification              | Rajveer Shastri, et al.                | 2015



Description of files
--------------------

- All code is written in python3

Non-Python files:

filename                          |  description
----------------------------------|------------------------------------------------------------------------------------
README.md                         |  Text file (markdown format) description of the project.

Python scripts files:

filename                          |  description
----------------------------------|------------------------------------------------------------------------------------
fetch_oeis_database.py            |  Fetch and refresh data from the remote OEIS database to a local sqlite3 database.

Python modules:

filename                          |  description
----------------------------------|------------------------------------------------------------------------------------
fraction_based_linear_algebra.py  |  Perform matrix inversion without loss of precision using the Fraction type.



# eeg_main.py

Keras implementation of Zhang et al(2018), "EEG-based Intention Recognition from Spatio-Temporal Representations via Cascade and Parallel Convolutional Recurrent Neural Networks" for EEG motar imagery classification on PhysioNet data (https://www.physionet.org/pn4/eegmmidb/). Stacked CNN and RNN were applied on time-distributed sliding windows of raw EEG data.

# eeg_preprocessing.py

This contains useful preprocessing steps to implement spatio-temporal pattern recognition on raw eeg data. Based on Scikit-learn and MNE pacakges.

# eeg_import.py

Functions defined to extract data from .edf file format using MNE package.

# eeg_data_downloads.py

Executing this code will generate folders and start downloading PhysioNet data into them.

# eeg.ipython

Jupyter notebook style

# Reference 

For the convenience of reading, I collected some basic and important papers about EEG processing.
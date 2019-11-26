# EEG-Literature

Prediction
----------
* [(Oct 2019) A Review on EEG Based Epileptic Seizure Prediction Using Machine Learning Techniques](https://link.springer.com/chapter/10.1007%2F978-3-030-30465-2_43)
* [(Oct 2019) Efficient Epileptic Seizure Prediction Based on Deep Learning](https://ieeexplore.ieee.org/document/8765420)
  * Dataset: CHB-MIT
  * Deep Convolutional Autoencoder + Bi-LSTM
  * Patient specific
* [(Oct 2019) Using Deep Learning and Machine Learning to Detect Epileptic Seizure with Electroencephalography (EEG) Data](https://arxiv.org/pdf/1910.02544.pdf)
  * Dataset: UCI
  * Training:Testing = 8:2
  * Good comparison of different ML and DL models
  * *on arxiv -- not reviewed*

Classification
--------------
* [(March 2019) A Novel Independent RNN Approach to Classification of Seizures against Non-seizures](https://arxiv.org/pdf/1903.09326.pdf)
  * Datasets: Bonn; CHB-MIT
  * Useful summary of related works
  * Training:Validating:Testing = 70:15:15
  * Develops IndRNN method - outperforms their implementation of LSTM and CNN approaches
  * Needs many more samples than traditional ML methods (long time span) 
  * Classification not prediction (realtime prediction using IndRNN is intended future work)
  * *on arxiv -- not reviewed*
* [(Sept 2017) Seizure Classification From EEG Signals Using Transfer Learning, Semi-Supervised Learning and TSK Fuzzy System](https://ieeexplore.ieee.org/document/8024036)  
  * Dataset: Bonn  
  * Introduces TSK method: not statistically better than other ML techniques, but output is more interpretable - generates "fuzzy rules" which can be written in english ``IF signal in frequency band 1 is High`` etc.
  * EEG data available: [link](http://epileptologie-bonn.de/cms/front_content.php?idcat=193&lang=3&changelang=3)
  * Classifies whether a patient is epileptic or not (easier problem)
* [(2016) Learning Robust Features using Deep Learning for Automatic Seizure Detection](http://proceedings.mlr.press/v56/Thodoroff16.html)
  * Dataset: CHB-MIT
  * 3D probe positions -> 2D points -> FFT, 3 bin RGB -Cubic Interpolation-> 2D images
* [(August 2015) Adversarial Representation Learning for RobustPatient-Independent Epileptic Seizure Detection](https://arxiv.org/pdf/1909.10868.pdf)
  * Adversarial method to be patient independent (i.e. not dependent on age and gender) 

Datasets
--------
* [CHB-MIT](https://physionet.org/content/chbmit/1.0.0/)
  * 22 humans: 5 males 3-22, 17 females 1.5-19
  * start and end of seizure is annotated
* [UCI](https://archive.ics.uci.edu/ml/datasets/Epileptic+Seizure+Recognition)
  * 500 humans
  * 23.5 seconds each
  * states labelled as:
    1. Recording of seizure activity
    2. They recorder the EEG from the area where the tumor was located 
    3. Yes they identify where the region of the tumor was in the brain and recording the EEG activity from the healthy brain area 
    4. eyes closed, means when they were recording the EEG signal the patient had their eyes closed
    5. eyes open, means when they were recording the EEG signal of the brain the patient had their eyes open
* [Bonn](http://ntsa.upf.edu/downloads/andrzejak-rg-et-al-2001-indications-nonlinear-deterministic-and-finite-dimensional)
  * 5 humans
  * A-E sets of 100 single channel EEGs, only set E contains seizures
  * Some preprocessing/filtering of data 
* [TUH EEG](https://www.isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml)
  * 316 humans
* [IEEG.org](https://www.ieeg.org)
  * Collection of many data sets
  * Mostly animals (?)
  * Don't know which ones are annotated

More Papers
-----------
* [A fuzzy classifier based detection for epileptic seizure signals](https://ieeexplore.ieee.org/document/8289771)
* [Do Features From Short Durational Segments Classify Epileptic EEG Signals Effectively?](https://ieeexplore.ieee.org/document/8629837)
* [Automated Epilepsy Diagnosis Using EEG With Test Set Evaluation](https://ieeexplore.ieee.org/document/8705361)
* [A Novel Double-Index-Constrained, Multi-View, Fuzzy-Clustering Algorithm and its Application for Detecting Epilepsy Electroencephalogram Signals](https://ieeexplore.ieee.org/document/8778649)
* [A Novel Synthetic CT Generation Method Using Multitask Maximum Entropy Clustering](https://ieeexplore.ieee.org/document/8811481)
* [A Survey on Transfer Learning](https://ieeexplore.ieee.org/document/5288526)
* [Collaborative Filtering for Brain-Computer Interaction Using Transfer Learning and Active Class Selection](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0056624)
* [Domain Adaptation via Transfer Component Analysis](https://ieeexplore.ieee.org/document/5640675)
* [Knowledge-Leverage-Based Fuzzy System and Its Modeling](https://ieeexplore.ieee.org/abstract/document/6263294)
* [Knowledge-Leverage-Based TSK Fuzzy System Modeling](https://ieeexplore.ieee.org/document/6502723)
* [Large margin transductive transfer learning](https://dl.acm.org/citation.cfm?id=1646121)
* [Transfer learning and active transfer learning for reducing calibration data in single-trial classification of visually-evoked potentials](https://ieeexplore.ieee.org/document/6974353)
* [Seizure Prediction by Graph Mining, Transfer Learning, and Transformation Learning](https://link.springer.com/chapter/10.1007/978-3-319-21024-7_3)
* [Applying Deep Learning for Epilepsy Seizure Detection and Brain Mapping Visualization](https://dl.acm.org/citation.cfm?id=3241056)
* [Optimized Deep Learning for EEG Big Data and Seizure Prediction BCI via Internet of Things](https://www.computer.org/csdl/journal/bd/2017/04/08094871/13rRUxly97y)

General notes
-------------
### Performance evaluation methods
* number of correctly predicted testing data / number of total testing data
* Friedman test + Holm's post hoc test


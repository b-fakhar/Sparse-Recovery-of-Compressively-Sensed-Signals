# Data-Compression
### Project Objective 
Develop an apply an optimization algorithm for data compression. The optimization algorithm based on L0-minimization is developed with the goal of: (1) improving the speed and quality recovery of the state-of-the-art sparse recovery MAX FS L0-minimization algorithms, and (2) improving the compression ratio of the well-known Compressive Sensing (CS) sparse recovery methods.  

### Challenges 
The data explosion in the digital age has created a demand in proposing strategies to manage data acquisition, transmission and data storage. CS is a widely used technique in data compression. However, the well-known sparse recovery algorithms can not handle highly compressed data. Therefore, there is a need to introduce an optimization algorithm that can handle high compression ration while providing high quality recovered data. 

### Achievements
According to the experimental results, the introduced algorithm

- Requires less number of measurement, which leads to higher compression, compared to the well-known CS sparse recovery methods such as Basis Pursuit (BP), Orthogonal Matching Pursuit (OMP), Matching Pursuit (MP), Smoothed-L0 (SL0).
- Provides  higher  fidelity  recovered  data  even though  their  solutions  are  sparser  than  those  of  CS  conventional  sparse recovery methods.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
###### Some details of the experimental setup are summarised in below. For more detail refer to our papers titled "Maximum Feasible Subsystem Algorithms for Recovery of Compressively Sensed Speech", "MAXimum Feasible Subsystem Recovery of Compressed ECG Signals", and "Recovery of Noisy Compressively Sensed Speech via Modified Maximum Feasible Subsystem Algorithm".

### Datasets

Two set of datasets are considered in this project to evaluate the performance of the newly developed algorithm.

- A total of 47 ECG signals that contain 22 women and 25 men at different age groups are taken from the MIT-BIH Arrhythmia Database (http://www.physionet.org/physiobank/database/mitdb).  A total of 18 selected ECG records (104, 107, 111, 112, 115, 116, 118, 119, 201, 207, 208, 209, 212, 213, 214, 228, 231, and 232) are pathologically significant. Digitization of the records was done at a rate of 360 samples/second per channel over a range of 10 mV with 11-bit resolution. For the analysis presented in this project, the first 3600 samples from each ECG signal are considered. Then, ECG signals are divided into segments of length n = 360, each of which contains at least one ECG cycle. Consequently, 47 ECG signals each comprised of 10 segments of length n = 360 are used in the experiments. In the following figure, a sample segment of a “pathologically significant” signal from the MIT-BIH Arrhythmia Database signal "104m' is presented. The segment contains one ECG cycle.  

![ECGsegment](https://user-images.githubusercontent.com/59096353/114275819-f9ad8a00-99f1-11eb-9ed7-35547d9a60bd.jpg)


- Speech inputs are drawn from the TIMIT database that includes time-aligned orthographic, phonetic and word transcriptions and speech waveforms sampled at 16kH. This well-known database has a total of 6300 sentences, 10 sentences spoken by each of 630 speakers, 438 male and 192 female, from 8 major dialect regions of the United States. 96 examples, 48 male and 48 female speakers, are used, covering all 8 dialect regions and all 3 types of sentences. The silent portions of a signal contain no useful information, so removing them decreases processing time and increases recovery accuracy. In our experiments, the silent parts of each input speech signal are removed based on the word transcription information in the TIMIT database.

### Tools/Software
Python, MATLAB, MOSEK, Latex.

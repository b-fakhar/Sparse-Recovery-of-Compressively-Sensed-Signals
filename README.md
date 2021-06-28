# Sparse Recovery of Compressively Sensed Signals
## Project Objective 
Develop and apply an optimization algorithm for sparse recovery to recover more highly compressed speech and ECG signals with greater quality. 
## Challenges 
The data explosion in the digital age has created a demand in proposing strategies to manage data acquisition, transmission and data storage. Compressive Sensing (CS) is a widely used compression technique with the two main phases (1) signal acquisition and (2) Sparse signal recovery. In CS like other compression techniques, higher compression is desired. To recover a highly compressed signal with high quality, the critical sparsity of a CS sparse recovery algorithm must be large enough. The well-known CS sparse recovery algorithms can not handle highly compressed data. Therefore, there is a need to introduce an optimization algorithm that can handle high compression ratio while providing high quality recovered signal. 

## Achievements
According to the experimental results, the introduced algorithm

- Requires less number of measurement, which leads to higher compression, compared to the well-known CS sparse recovery methods such as Basis Pursuit (BP), Orthogonal Matching Pursuit (OMP), Matching Pursuit (MP), Smoothed-L0 (SL0).
- Provides  higher  fidelity  recovered  data  even though  their  solutions  are  sparser  than  those  of  CS conventional sparse recovery methods.

## Related Pulications
### Refereed Journal Publications

##### •	F. F. Firouzeh, S. Rajan, J. W. Chinneck, " Fast Maximum Feasible Subsystem Algorithm for Recovery of Compressively Sensed ECG,” Submitted to IEEE Transactions on Instrumentation and Measurement.
##### •	F. F. Firouzeh, J. W. Chinneck and S. Rajan, "Maximum Feasible Subsystem Algorithms for Recovery of Compressively Sensed Speech," IEEE Access., vol.8, no. 1, pp. 82539-82550, 2020. Accessed on: May. 15, 2020. [Online]. Available doi: 10.1109/ACCESS.2020.2990155.

### Refereed Conference Publication

##### •	F. F. Firouzeh, S. Rajan, J. W. Chinneck, “MAXimum Feasible Subsystem Recovery of Compressed ECG Signals,” 2020 IEEE International Symposium on Medical Measurements and Applications (MeMeA), Bari, Italy, June 1-3, pp. 1-5, 2020.

---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
###### Some details of the experimental setup are summarised in below. For more detail refer to the papers menttioned above.

## Datasets

Two set of datasets are considered in this project to evaluate the performance of the newly developed algorithm.

- A total of 47 ECG signals that contain 22 women and 25 men at different age groups are taken from the MIT-BIH Arrhythmia Database (http://www.physionet.org/physiobank/database/mitdb).  A total of 18 selected ECG records (104, 107, 111, 112, 115, 116, 118, 119, 201, 207, 208, 209, 212, 213, 214, 228, 231, and 232) are pathologically significant. Digitization of the records was done at a rate of 360 samples/second per channel over a range of 10 mV with 11-bit resolution. For the analysis presented in this project, the first 3600 samples from each ECG signal are considered. Then, ECG signals are divided into segments of length n = 360, each of which contains at least one ECG cycle. Consequently, 47 ECG signals each comprised of 10 segments of length n = 360 are used in the experiments. In the following figure, a sample segment of a “pathologically significant” signal from the MIT-BIH Arrhythmia Database signal "104m' is presented. The segment contains one ECG cycle.  

![ECGsegment](https://user-images.githubusercontent.com/59096353/114275819-f9ad8a00-99f1-11eb-9ed7-35547d9a60bd.jpg)


- Speech inputs are drawn from the TIMIT database (https://abacus.library.ubc.ca/dataset.xhtml?persistentId=hdl:11272.1/AB2/SWVENO) that includes time-aligned orthographic, phonetic and word transcriptions and speech waveforms sampled at 16kH. This well-known database has a total of 6300 sentences, 10 sentences spoken by each of 630 speakers, 438 male and 192 female, from 8 major dialect regions of the United States. 96 examples, 48 male and 48 female speakers, are used, covering all 8 dialect regions and all 3 types of sentences. The silent portions of a signal contain no useful information, so removing them decreases processing time and increases recovery accuracy. In our experiments, the silent parts of each input speech signal are removed based on the word transcription information in the TIMIT database.

### Tools/Software
Python, MATLAB, MOSEK, LaTeX.

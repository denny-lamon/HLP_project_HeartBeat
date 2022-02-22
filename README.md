# HLP_project_HeartBeat
The data is provided in .txt files. During this study, two healthy subjects were involved with their informed consent. The first dataset (center_sternum.txt) was recorded on one subject, while all the other datasets (1_Stave_supine_static.txt, 2_Mattress_supine.txt, 3_Subject_sitting_chair.txt, 4_Chest_sweater.txt, 5_Under_chair.txt) were recorded on the second subject. 

# Assignment
Data preparation:

1.1. Load the txt files and select only the columns you are interested in, in order to do a complete data analysis (e.g. Log Freq, AccX, ... )

1.2. Plot selected data as a function of time and choose a proper time window over which to perform the analysis. Pay attention on the time representation and the measurement unit.

1.3. In order to do a proper job, decide whether to consider some particular axis or some combination of them as well as derived features for the next step of the task. Motivate your choice.

Time and frequency analysis:

2.1. Statistical analysis: provide a statistical description of the chosen dataset. Statistical descriptors includes for example mean, median, variance, standard deviation, 25th and 75th percentiles, and correlation coefficients. Investigate what could be the most interesting descriptors for this type of data, motivating the choices.

2.2. Fourier Analysis: Perform a frequency analysis of the data. Look at the spectrum and explain what you see. Use the Fourier analysis to properly design the filters in the following step.

Filter:

Implement your own filter, trying to extrapolate the heart rate signal. Hints:

(a) Directly from Fourier Analysis, look for the most interesting frequency band.

(b) Choose the appropriate Lowpass/Bandpass/Highpass filter.

(c) Explore another methods by yourselves.

Remember to always motivate your choice.

Metrics:

4.1. Heart Beat Per Minute (BPM): extrapolate BPM, make an histogram of the result. Does it follow a particular distribution?

4.2. Heart Rate Variability (HRV): extrapolate HRV, explain why this parameter is important, and plot the results.

Optional: Elaborate a simple algorithm to extrapolate the heart rate even when the filter fails (e.g. look for a particular threshold...).
Conclusion:

Summarise the obtained results, and specifically make a comparison between the two files analysed. Highlight the limitations and the critical issues encountered during the work, motivating the most relevant contribution given by your solution.


# Index
- Data preparation (Lamon) 
  - Rough data | Calibration of the data | Columns selection
  - Acquisition time and sampling frequency | Sampling rate barplot
  - First data plots | Data selection
  - Axis projections
  - Data zoom in ( ∼ 2 seconds)
  - Vectors modules & Vectors modules ( ∼ 5 seconds)
  - Quaternions to angular coordinates | Quaternions plot |Breath frequency (FT)
  - Rotation coordinates plots ( ∼ 15 seconds) | 3D animation: quaternions
  
- Variables selections (Farina)
  - Computing FT and SNR
  - Signal to Noise Ratio of the FT
  - Statistical analysis
  - PCA Analysis
  - Fourier Analysis
  - Fitting of FFT: BPM and HRV estimation
  - Filters
  
- Antitrasforming: Heart Beat signal (Khiari) 
  - Antitransform FT with band-pass filter
  - Antitransform FT with band-pass + gaussian filters
  - Optional: extrapolating the Heart rate with a threshold
  
- Trials with other files (Lamon) 

- Final results and comparison

# Subdivision of the work 
Each of the three principal sections has been developed mainly by the person indicated above, but lots of contributions on code scripts and analysis ideas have been shared and are present in many of the the different parts of the code. 


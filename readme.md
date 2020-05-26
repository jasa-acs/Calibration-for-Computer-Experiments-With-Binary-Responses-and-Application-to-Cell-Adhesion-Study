# Calibration for Computer Experiments With Binary Responses and Application to Cell Adhesion Study

# Author Contributions Checklist Form

## Data

### Abstract

The full data consists of simulated and experimental data for the T cell adhesion experiments, including their parameter values and binary outputs. 

File "labdata.txt" contains the (lab) experimental data for the T cell adhesion experiments. Two control variables, "tc" and "tw", are in the first and second columns of the data, and the corresponding binary output of each combination of the two control variables, "y", is in the third column. There are 272 samples (i.e., 272 rows).

File "simdata.txt" contains the simulation data for the T cell adhesion experiments. Six control variables, "tc", "tw", "kc", "kf", "kr", and "krx", are in columns 1-6 of the data, and the corresponding binary output of each combination of the six control variables, "ys", is in the 7th column. There are 1200 samples (i.e., 1200 rows).




### Availability 

Both simulated and experimental data are publicly available at https://bitbucket.org/chihli/binarycalibration/.


### Description 

Permissions: Dataset simulated using internal code and generated from lab experiments
Licensing information: -----
Link to data: https://bitbucket.org/chihli/binarycalibration/
Data provenance, including identifier or link to original data if different than above: -----
File format: .txt 
Metadata (including data dictionary): -----
Version information: -----



## Code

### Abstract

The code folder consists of R packages and the code used for generating results. The code is completely written in R.

File "simulation_2d.R" can reproduce Tables 1 and Figures 3-4, which is running simulated examples of 2-dimensional computer experiments and comparing the proposed method with a naive approach.

File "simulation_5d.R" can reproduce Tables 2, which is running simulated examples of 5-dimensional computer experiments.

File "realdata.R" analyzes the T cell adhesion experiments based on the proposed calibration method in the paper. This file can reproduce Figures 5-7, which illustrates the raw data, fitted surface for the physical experiments, sensitivity analysis for the computer experiments, and the comparison of the fitted models from the physical and computer experiments. This file also returns the estimated calibration parameters and their corresponding standard deviations for the T cell adhesion experiments.


### Description

How delivered: R package and code
Licensing information: MIT License
Link to code/repository: https://bitbucket.org/chihli/binarycalibration/
Version information: master+ afe4b6b


## Instructions for Use

Supporting  software  requirements:  R (>=  3.2.4):
kernlab (>=0.9-25)
lhs (>=0.15)
sensitivity (>=1.15.2)
numDeriv (>=2016.8-1)
lattice (>=0.20-35)
calibrateBinary (>=0.2)
ggplot2 (>=3.0.0)
randomForest (>=4.6-14)
Set the working directory as the path of the folder we provided, then run the files “simulation_2d.R”, “simulation_5d”, and “realdata.R”.


### Reproducibility 

Tables 1-2, Figures 3-7, and the estimated calibration parameters and their corresponding standard deviations in Section 5.


Tables 1-2 and Figures 3-4 can be reproduced by running “simulation_2d.R” and  “simulation_5d”. Figures 5-7, the estimated calibration parameters and their corresponding standard deviations can be reproduced by running “realdata.R”.

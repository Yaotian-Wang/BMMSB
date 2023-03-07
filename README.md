# A Variational Bayesian Approach to Identifying Whole-Brain Directed Networks with fMRI Data

## Description

This toolbox *BMMSB* contains the functions we developed for our proposed Bayesian method in our paper *A Variational Bayesian Approach to Identifying Whole-Brain Directed Networks with fMRI Data*, accepted by *The Annals of Applied Statistics*. Readers can use this toolbox to reproduce the results in our simulation studies (Section 4) and modify the scripts to analyze their real data without difficulty. 

## Installation

Our toolbox *BMMSB* is published as a Matlab package. 

## Usage

Detailed guidelines on using these functions can be found in BMMSB\_manual.pdf.

- BMMSB\_ContPnl\_ms.m: The control panel of our proposed Bayesian method with the mixed-membership stochastic blockmodel prior (BMMSB). It shows how to analyze our simulated data step by step and serves as an example of using our toolbox;
- BMMSB\_VB\_par\_ms.m: The primary function of our variational Bayesian algorithm, which is developed for estimating our proposed Bayesian model;
- MARSS\_ContPnl.m: The function for estimating state functions through a standard multivariate autoregressive state-space (MARSS) model;
- BMMSB\_Omega.m, BMMSB\_P.m: Functions for the posterior inference that we illustrated in Section 3.1; 
- BMMSB\_BIC.m: The function for choosing hyperparameters;
- BMMSB\_generate\_Simu.m: The function generates simulated data in our simulations studies (Section 4). It depends on the [SPM12 toolbox](https://www.fil.ion.ucl.ac.uk/spm/software/spm12/). 


## Data
The 995 subjects' resting-state fMRI data we analyzed in our paper are from the [Human Connectome Project (HCP)](https://db.humanconnectome.org/). 

This toolbox does not contain the 1000 subjects' simulated data that we analyzed in our paper due to the large file size. Instead, it contains the true network structure of our simulated data (BMMSB\_A\_true\_S.mat). Users can generate the same simulated data that we analyzed in our paper by the function BMMSB\_generate\_Simu.m.

## Reference
Yaotian Wang, Guofen Yan, Xiaofeng Wang, Shuoran Li, Lingyi Peng, Dana L Tudorascu, and Tingting Zhang (2022).  A Variational Bayesian Approach to Identifying Whole-Brain Directed Networks with fMRI Data, *The Annals of Applied Statistics*, accepted. 

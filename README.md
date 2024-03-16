# Brain Amplification Mechanism - Analysis Replication Guide

This repository contains the Python code and instructions necessary to replicate the analysis presented in the Brain Amplification Mechanism paper using the Osyris Replicate python package. The analysis focuses on understanding balanced amplification in neural networks through a series of computational steps and visualizations.

## Steps to Replicate the Analysis

### Getting started
Install and import the package
**Code:** `pip install osreplicate`
**Code:** `from osreplicate import Paper`

### Access the paper you want to replicate
Provide the papers alias to start analyzing

**Code:** `analysis = Paper('uc/Balanced Amplification')`

### Get the datasets
Locally download any available datasets associated with this paper

**Code:** `analysis.get_data()`

### Replicate the paper
Automatically run the full analysis on the available datasets and reproduce the figures from the paper
`analysis.run()`

### Step 1: Mix and match      
Access core analysis methods from to the paper\
`analysis.linear_firing_rate_model(tau, r, W, I)`\
`analysis.decompose_network_activity_and_input(P, r_t, I_t)`\
`analysis.construct_connectivity_matrix(W_EE, W_EI, W_IE, W_II)`\
`analysis.balanced_amplification_model(w, k_I)`\
`analysis.plot_cross_covariance(cross_covariance, max_lag)`

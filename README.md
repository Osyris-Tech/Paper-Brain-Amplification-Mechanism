# Brain Amplification Mechanism - Analysis Replication Guide

This repository contains the Python code and instructions necessary to replicate the analysis presented in the Brain Amplification Mechanism paper. The analysis focuses on understanding balanced amplification in neural networks through a series of computational steps and visualizations.

## Steps to Replicate the Analysis

### Step 1: Linear Firing Rate Model for Balanced Amplification
Implement the linear firing rate model to understand how firing rates change over time based on synaptic connectivity and external inputs.

**Code:** `linear_firing_rate_model(tau, r, W, I)`

### Step 2: Decomposition of Network Activity and Input
Decompose network activity and inputs into basis patterns to analyze network dynamics more granularly.

**Code:** `decompose_network_activity_and_input(P, r_t, I_t)`

### Step 3: Basis Pattern Dynamics and Hebbian Amplification
Explore how each basis pattern's amplitude evolves over time, influenced by the network's eigenvalues.

**Code:** `compute_pattern_dynamics(tau, w_eigenvalues)`

### Step 4: Connectivity Matrix Structure in Biological Networks
Understand the network's connectivity matrix structure, distinguishing between excitatory and inhibitory connections.

**Code:** `construct_connectivity_matrix(W_EE, W_EI, W_IE, W_II)`

### Step 5: Simple Model of Balanced Amplification
Analyze a simplified model that illustrates balanced amplification in networks with excitatory and inhibitory neuron populations.

**Code:** `balanced_amplification_model(w, k_I)`

### Step 6: Decomposition and Dynamics of Sum and Difference Modes
Study how sum and difference modes interact and evolve within the network.

**Code:** `sum_difference_modes_dynamics(tau, r_E_t, r_I_t, w_plus, w_FF)`

### Step 7: Firing Rate Response to External Input
Investigate how excitatory neuron populations respond to external inputs in Hebbian and balanced network models.

**Code:** Functions `effective_decay_time(tau, w)` and `balanced_network_dynamics(tau, r_E_t, r_I_t, w_plus, w_FF)`

### Step 8: Spatially Extended Networks and Balanced Amplification
Extend the analysis to spatially extended networks, examining how the connectivity matrix influences pattern amplification.

**Code:** `spatial_network_amplification(W_E, W_I)`

**Visualization:** Implement vibrant color plots to visualize the connectivity matrix and eigenvalue distribution.

### Step 9: Validation with Detailed Biophysical Model
Validate the balanced amplification principles using a detailed biophysical model, analyzing correlation and autocorrelation.

**Code:** `plot_results(correlation_coefficients, autocorrelation_function)`

### Step 10: Cross-Covariance Analysis in Spiking and Linear Models
Analyze the relationship between sum and difference modes through cross-covariance functions in both spiking and linear models.

**Code:** `plot_cross_covariance(cross_covariance, max_lag)`

## How to Use This Repository

1. Clone the repository to your local machine.
2. Install the required Python libraries: `numpy` and `matplotlib`.
3. Follow the steps sequentially, executing the provided Python functions for each analysis step.
4. Use the provided plotting functions to visualize the results after each relevant step.

## Contribution

Feel free to fork this repository and submit pull requests if you have suggestions for improvements or have found issues.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

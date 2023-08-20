# Module 20 Neural Networks: Deep Learning

## Overview of the Analysis

Evaluate historical data for a nonprofit foundation, Alphabet Soup, to help identify funding applicants with the highest of success.

Features:
* Application Type
* Affiliation
* Classification
* Use Case
* Organization
* Status
* Income Amount
* Special Considerations
* Ask Amount
  
Target:
* Is Succesful

## Approach

Build a Neural Network to classify applicants on the likelihood of success.
* Preprocess the Data: ensure all data is usable by model
* Compile, Train, and Evaluate the Model: build a model based on historical data and measure accuracy
* Optimize the Model: change key parameters to achieve increased accuracy

## Results

* Neural Network: Original Data
  * Hidden Layers: 2
  * Hidden Layer 1: 80 Neurons, ReLu Activation
  * Hidden Layer 2: 30 Neurons, ReLu Activation
  * Accuracy: 72.76%

* Optimization 1: Add Hidden Layer and Increase Neurons
  * Hidden Layers: 3
  * Hidden Layer 1: 80 Neurons, ReLu Activation
  * Hidden Layer 2: 50 Neurons, ReLu Activation
  * Hidden Layer 3: 30 Neurons, ReLu Activation
  * Accuracy: 72.52%
 
* Optimization 2: Change Activation and Increase Neurons
  * Hidden Layers: 3
  * Hidden Layer 1: 80 Neurons, tanh Activation
  * Hidden Layer 2: 80 Neurons, tanh Activation
  * Hidden Layer 3: 80 Neurons, tanh Activation
  * Accuracy: 72.54%

* Optimization 3: Drop Variables
  * Dropped: Status, Special_Considerations
  * Hidden Layers: 3
  * Hidden Layer 1: 80 Neurons, ReLu Activation
  * Hidden Layer 2: 80 Neurons, ReLu Activation
  * Hidden Layer 3: 80 Neurons, ReLu Activation
  * Accuracy: 72.66%

## Summary

Each model achieved similar results of approximatley 72%.  To achieve a desired 75% accuracy we may attempt a differnt Machine Learning model or continue to tweek the existing Neural Network model through additional layers, neurons, modifying activation, and/or dropping columns wtih little contribution to the accuracy.


# Peak Identifier

The purpose of this project was to develop a machine-learning model that could identify target peaks in microchip electrophoresis (MCE) traces of antibodies. A common issue with MCE traces is that they will often detect contaminants or fragments of antibodies. These extraneous peaks make analyzing MCE traces tedious and require manual analysis of each trace. The development of a machine learning model would maximize the efficiency of the analysis of these traces.

## Project Goals
Problem: MCE instruments are not consistent
- Evaluation of molecule traces requires manual analysis of traces
- Identifying target peaks is difficult with variations in retention times

![image](https://github.com/kyshu11027/PeakIdentifier/assets/96274909/ba299832-5132-4d51-ae08-84db929f82d9)

Goal: Automated Target Peak Identifier

## Need for a Classifier
- Input: Trace window located at expected target peak location
- This iteration of this project would differentiate good, bad, and complicated peaks
- Output: Does this window contain a good, bad, or complicated peak?

## Classification Methods

Traditional clustering failed, so we turned to dimensionality reduction and sparse coding.

# Sparse Coding Increased Performance
- Sparse coding is a form of dimensionality reduction
- Sparse coding takes a group of exemplar traces
- Evaluates each trace as a linear combination of these exemplar traces
- Classify traces based on their linear combinations
- Increased performance!

# Different Classification Methodologies Tested
- K-Nearest Neighbors
- Naïve Bayes
- Random Forest
- Logistical Regression
- Decision Tree


# Code description

This repository contains the codes necessary to generate the main results described in our paper "Machine Learning for the ECG Diagnosis and Risk Stratification of Occlusion Myocardial Infarction at First Medical Contact".

The code in the main.ipynb file loads the derivation and external validation datasets, trains a calibrated random forest (RF) classifier and tests its performance on an internal testing set and an external validation set. Risk scores are provided for all the patients during the training, internal testing and external validation phases, and the cutoffs defined in the paper are used to distinguish three risk groups/levels: low, intermediate and high risk. 

The code sections are as follows:
\begin{itemize}
  \item Importing relevant libraries and packages
  \item Loading the data files for the derivation and external validation cohorts (and displaying some of the data)
  \item Data splitting (into training and internal testing for the derivation cohort) and preprocessing (missing data imputation and data z-score normalization)
  \item Defining and calibrating the RF classifier
  \item Defining functions for: ROC curve plotting, results stratification into risk groups, and Shapley explainability plot display.
  \item Training
  \item Displaying the risk groups count for training
  \item Internal testing
  \item Displaying the risk groups count for internal testing
  \item External validation
  \item Displaying the risk groups count for external validation
\end{itemize}

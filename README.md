# Credit Risk Analysis

## Overview

The following is an analysis of balanced accuracy score, precision, and recall of six different algorithms trained to predict credit risk based on LendingClub credit data. Methods tested include oversampling by random oversampling and synthetic minority oversampling technique (SMOTE), undersampling using cluster centroid undersampling, combination over and undersampling using the SMOTE and Edited Nearest Neighbors (SMOTEENN) algorithm, and the Balanced Random Forest and EasyEnsemble algorithms, two machine learning models designed to reduce bias.

## Results

### Random Oversampling

* 0.65 balanced accuracy score
* 0.01 precision
* 0.61 recall

![](resources/random_oversampling.png)

### SMOTE

* 0.62 balanced accuracy score
* 0.01 precision 
* 0.61 recall 

![](resources/SMOTE.png)

### Cluster Centroid Undersampling

* 0.51 balanced accuracy score
* 0.01 precision 
* 0.62 recall 

![](resources/cluster.png)

### SMOTEENN

* 0.61 balanced accuracy score
* 0.01 precision 
* 0.69 recall 

![](resources/SMOTEENN.png)

### Balanced Random Forest

* 0.79 balanced accuracy score
* 0.04 precision 
* 0.67 recall 

![](resources/random_forest.png)

### EasyEnsemble

* 0.92 balanced accuracy score
* 0.07 precision
* 0.91 recall

![](resources/easy_ensemble.png)

## Summary

Among the models tested, all of the over/undersampling models performed similarly with balanced accuracy scores between 0.51 (cluster centroid undersampling) and 0.65 (random oversampling). All of these models had a precision of 0.01 and recalls between 0.61 (random oversampling and SMOTE) and 0.69 (SMOTEENN), and therefore none of these models would be recommended. The ensemble models performed better in all metrics, with the EasyEnsemble outperforming the Balanced random forest in all aspects. The EasyEnsemble had the best balanced accuracy score (0.92) and a recall of 0.91, indicating that 91% of true high risk loans would be identified. For this reason, it would recommended to use the EasyEnsemble model. 

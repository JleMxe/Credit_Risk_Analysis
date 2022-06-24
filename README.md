# Credit Risk Analysis

# Overview
The purpose of this analysis is to explore various models and resampling techniques to determine an effective way to assess credit worthiness (credit risk). 

# Results
## Methods used with results shown below:

### Random Over Sampling
![Credit Risk Analysis](/pictures/RandomOversampler.png)
- Balanced Accuracy Score was = .64
- Precision
  - High Risk = .01
  - Low Risk = 1.0
- Recall
  - High Risk = .72
  - Low Risk = .56

### SMOTE Over Sampling
![Credit Risk Analysis](/pictures/SMOTEOversampler.png)
- Balanced Accuracy Score was = .66
- Precision
  - High Risk = .01
  - Low Risk = 1.0
- Recall
  - High Risk = .62
  - Low Risk = .69

### Under Sampling
![Credit Risk Analysis](/pictures/UnderSampling.png)
- Balanced Accuracy Score was = .54
- Precision
  - High Risk = .01
  - Low Risk = 1.0
- Recall
  - High Risk = .69
  - Low Risk = .40

### Combination Sampling
![Credit Risk Analysis](/pictures/CombinationSampling.png)
- Balanced Accuracy Score was = .67
- Precision
  - High Risk = .01
  - Low Risk = 1.0
- Recall
  - High Risk = .73
  - Low Risk = .6

### Balanced Random Forest Classifier
![Credit Risk Analysis](/pictures/BalancedRandomForestClassifier.png)
- Balanced Accuracy Score was = .79
- Precision
  - High Risk = .03
  - Low Risk = 1.0
- Recall
  - High Risk = .7
  - Low Risk = .87

### Easy Ensemble Classifier
![Credit Risk Analysis](/pictures/EasyEnsembleClassifier.png)
- Balanced Accuracy Score was = .93
- Precision
  - High Risk = .09
  - Low Risk = 1.0
- Recall
  - High Risk = .92
  - Low Risk = .94

# Summary

The summary below compliles the results into a more easily read format.
![Credit Risk Analysis](/pictures/summary.png)


The conclusion based the above results, there is a very clear preferred choice for methodology to be employed and that is the Easy Ensemble Classifier model. It had the highest Balanced Accuracy Score at .93. It also had the highest Precision of all the explored methods. High Risk Precision was .09 (the next closest was the Balanced Random Forest Classifier at .03) and a Low Risk Precision of 1.0 (this was the same across all methods explored). Furthermore, it had the highest Recall at .7 for High Risk and .87 for Low Risk (these were also the closest together). By all explored metrics, Easy Ensemble Classifier is the best choice.


# tf_bayesian
Transformers Can Do Bayesian Inference
Prior-Data Fitted Networks


## Overview

1. Bayesian methods are widely used in science and industry and can provide both optimal solutions, uncertainty estimates, and interpretability, but can be computationally intractable or unsolvable.
2. Bayesian methods can be used for machine learning, but see above. If they could be made to work they might beat current methods and sidestep the No Free Lunch problem. 
3. One of the most useful parts of Bayesian modeling, the prior, often gets wasted because it is too difficult to calculate them.
4. Deep learning has been used to solve bayesian problems, but success has been limited.
5. In possibly groundbreaking work, the authors show how a kind of self-supervised learning (using artificial generated data) can be used build priors and caclculate posterior probabilities using a Transformer network. 
6. In sample work, this approach outperformed XGBoost and CatBoost, and provided meaningful uncertainty, while training more than 5,000 times faster (from 20 hours to 13 seconds)!
7. More exploration needs to be done to see if the promised holds more generally. 

### Predicting Outcomes from Tabular Datasets

From their paper, Muller, Hollmann, Pineda, Grabocka, and Hutter describe how they pretrain on a universe of Bayesian Neural Network priors:

![image](https://user-images.githubusercontent.com/5521243/158394006-ce275df7-f618-4b95-b9da-4b0aa3bcc630.png)


## Discussion Topic 1

IF the findings in the paper generalize broadly, what impact could this have on future Machine Learning approaches?

## Discussion Topic 2

The approach described fits models 100-5,000 times faster than existing methods. What are some other possible advantages to the approach? What are some possible drawbacks? (HINT: Which is faster to score (or inference)--an XGBoost model or a large(ish) Transformer model)?

## Discussion Topic 3

The models provide excellent uncertainty calibration--they provide not just point estimates, but ranges of uncertainty that are close to true probabilities. How might that be helpful?


## Critical Analysis

In their comparison to machine learning methods (XGBoost and CatBoost), the authors note that they only analyzed datasets from MLBenchmark that were not missing data and that had fewer than 100 predictors, and further simplified the datasets to be balanced. They did not indicate whether their approach was limited to only datasets that met these criteria, or whether this was for expediency. If this is a limitation of the approach, this should have been highlighted. 

 

## Resource links

Original Article: https://arxiv.org/abs/2112.10510
Code and trained PFNs are released at https://github.com/automl/TransformersCanDoBayesianInference
Spaces for tabular models https://huggingface.co/spaces/samuelinferences/transformers-can-do-bayesian-inference

## Code demonstration

The code has not yet been made availalbe.

## Video Recording

Link to video recording.

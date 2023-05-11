# deep_learning_challenge

## Overview

A nonprofit named Alphabet Soup (AS) provides funding to many organizations the world over. This is a commendable endeavor, but AS wants a tool that helps them better select applicants with the highest chances of success. We have been tasked with creating a binary classifier, using neural networks, to help predict whether applicants will be successful or not. AS has given us a large dataset of past recipients of funding. The dataset includes many features which are assumed to have an affect on outcome as well as label data of successful or not successful.

## Results

* Data Processing
    - Target:
        * IS_SUCCESSFUL
    - Features:
        * APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL CONSIDERATIONS, ASK_AMT
    - Neither:
        * EIN, NAME
    
* Compiling, Training, Evaluating Model:
    - Neurons, Layers, Activation:
        * 1st Hidden Layer: 36 inputs nodes, 16 nodes (hidden), activation= relu
        * 2nd Hidden Layer: 8 nodes, activation= relu
        * Output Layer: 1 node, activation= sigmoid
        * Why: For this first attempt at the model I chose 16 nodes then 8 nodes for the hidden layers becuase the sum of those is equal to 2/3 the input nodes plus the output node. Relu functions were used becuase they are the default activation functions for hidden layers currently and thus a good place to start. Sigmoid is used for the output layer because you must use it when creating a binary classifier. It is a logistic function.
    - Target Model Performance Achieved???
        * No. 
    - Optimization Efforts:
        * Model 2 (Accuracy: 0.7239): added more nodes to the hidden layers (26, 16), more than the rule of thumb used in the original but still less than twice the number of input nodes (another rule of thumb)
        * Model 3 (Accuracy: 0.7243): kept the node change from model 2 and added a few more application types to the other bin in hopes of reducing the affect of outliers
        * Model 4 (Accuracy: 0.7211): kept all from above and added a third hidden layer with 8 nodes and a relu activation

## Summary

Overall the model did not hit it's target performance, even with optimization efforts. That said, ~ 72% accuracy in predicting successful applicants is still good in the grand scheme of things. I would recommend Alphabet Soup use model #3 and keep iterating with it to hopefully improve performance. Something that could really help here is to talk with the folks at Alphabet Soup and learn more about these features and their importance. Once that is better understand, possibly trim some more and also handle some possible outliers within features.
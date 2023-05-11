# deep_learning_challenge

## Overview

A nonprofit named Alphabet Soup (AS) provides funding to many organizations the world over. This is a commendable endeavor, but AS wants a tool that helps them better select applicants with the highest chances of success. We have been tasked with creating a binary classifier, using neural networks, to help predict whether applicants will be successful or not. AS has given us a large dataset of past recipients of funding. The dataset includes many features which are assumed have an affect on outcome as well as label data from successful or not successful.

## Results

* Data Processing
    - Targets:
        > APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL CONSIDERATIONS, ASK_AMT
    - Features:
        > IS_SUCCESSFUL
    - Neither:
        > EIN, NAME
    
* Compiling, Training, Evaluating Model:
    - Neurons, Layers, Activation:
        > 1st Hidden Layer: 36 inputs nodes, 16 nodes (hidden), activation= relu
        > 2nd Hidden Layer: 8 nodes, activation= relu
        > Output Layer: 1 node, activation= sigmoid
        > Why: For this first attempt at the model I chose 16 nodes then 8 nodes for the hidden layers becuase the sum of those is equal to 2/3 the input nodes plus the output node. Relu functions were used becuase they are the default activation functions for hidden layers currently and thus a good place to start. Sigmoid is used for the output layer because you must use it when creating a binary classifier. It is a logistic function.
    - Target Model Performance Achieved???
        > No. 
    - Optimization Efforts:
        >

## Summary
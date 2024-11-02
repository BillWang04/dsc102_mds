# Data Flow Systems

Usually RDBMS are really good, howver there are few things that need to be done that RDBMSs are pretty bad at.

- The 4 concerns are:
    - Developability: Custom data models and computations hard to program on SQL/RDBMSs, need for simpler APIs
    - Fault Tolerance: Need to scale to 1000s of machines; need for graceful handling of worker failure
    - Elasticity: Need to be able to easily upsize or downsize cluster size based on workload
    - Cost: Commercial RDBMSs licenses too costly; hired own software engineers to build custom new systems


## Map Reduce:

A programming model for parallel programs on sharded data + distributed system architecture

- The system handles data distribution, parallelization, fault tolerance under the hood
 Created by google

 Map reduce is a functional programming model, meaning that it first creates a paradigm of building computer programs using expressions and functions without mutating state and data. And then you pipeline the data into it.


 ## ML Features

 Umbrella term for many tasks dep. on type of ML model trained:
1. Recording and value conversions
    - Standardization
    - Binning
    - One hot Encoding
2. Joins and/or aggregates
    - Combing dataframes to find the best features
3. Feature interactions
    - g 
4. Feature selection
    - Select a subset
    - 
5. Dimensionality reduction
    - PCA
    - Spectrum Dimensionality
6. Temporal feature extraction
7. Textual feature extraction and embeddings
8. Learned feature extraction in deep learning

### Hyper-Parameter Tuning
Knobs for an ML model or training algorithm to control bias-variance tradeoff in a dataset-specific manner to make learning effective










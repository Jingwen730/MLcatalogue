# Catalogue of deep learning models 
Note: All models and training datasets are archived on our AWS SE bucket ml-catalogue.
## ML model with 5 mechanisms
### The original model [published](https://pubs.acs.org/doi/10.1021/acsmeasuresciau.2c00045)
1. 5 homogeneous mechanisms: E, EC, CE, ECE, DISP
2. ~5k training data for each mechanism
3. scan rates: linearly between 0.01 to 2 V/s
- Model: original paper model.zip
- Training data: secondcycle.zip
### Model with enlarged, linearly-sampled scan rates (06/10/2022)
1. scan rates: linearly between 0.01 to 10 V/s
- Model: linear 5 mech model.rar
- Training data: linear_5_training.rar
### Model with enlarged, logarithmically-sampled scan rates (06/10/2022)
1. scan rates: logarithmically between 0.01 to 10 V/s
- Model: log 5 mech model.rar
- Training data: log_5_training.rar
### Model with both linearly and logarithmically-sampled scan rates (06/10/2022)
1. scan rates: both linearly and logarithmically between 0.01 to 10 V/s
- Model: mix 5 mech model.rar
- Training data: should be the mixture of linear_5_training.rar and log_5_training.rar
## ML model with 9 mechanisms 
### 9 mechanisms ML model (09/20/2022)
1. 9 homogeneous and heterogeneous mechanisms: E, EC, CE, ECE, DISP, DL, EC', T, SR 
2. scan rates: linearly and logarithmically between 0.01 to 10 V/s
- Model: 9 mech model.rar
- Training data: 9_training_orig.rar
### 9 mechanisms ML model from Pranav (10/10/2022)
- Model: 9 mech model Pranav.rar
- Training data: forPranav.zip in aws s3 bucket pranavdatabucket
###  9 mechanisms ML model with modified EC training data (10/20/2022)
1. The EC data is replaced by EC1, which only includes EC inside the kinetic zoom (KO, KG, KE, KP)
- Model: 9 mech model modified EC.rar
- Training data: 9_training_newEC.rar

### 9 mechanisms ML model with modified 9 mechanisms training data (11/28/2022)
1. Untypical CV data of all mechanisms are manually removed.
- Model: To be trained
- Training data: 9_training_filter.rar

## Merge CV 
### Merged CV identification based on 9 mechanisms (11/28/2022)
- Training data: mergeCV_training.rar

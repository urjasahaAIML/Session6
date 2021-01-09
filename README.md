# Session6 Assignment Submission

## Link to Assignment
TODO: Describe the installation process

## Link to Validation Accuracy graph:
https://github.com/tapasML/Session6/blob/main/validation_accuracy.png

## Link to Loss curve graph:

## Link to mis classified images:
https://github.com/tapasML/Session6/blob/main/misclassified.png


## Details about the code:
5 model types are created for choice (1-5)
1. with L1 + BN
2. with L2 + BN
3. with L1 and L2 with BN
4. with GBN
5. with L1 and L2 with GBN


# Globals used
EPOCHS = 25
LAMBDA_1= 0.001  #L1 parameter, same as L2 weight decay. 
ghostGroups = 8 # number of 'Ghost' groups

# Details
Each choice (1-5) creates a loop for model and runs 25 epochs, saves the last epoch validation loss, accuracy statistics in global array
Misclassified images are captured only in last epoch (25th)
Regularization block defines the GhostNorm() function
Choice 4,5 (with GhostBN) is run with higher learning rate.
Dropout is not used



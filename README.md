# Supervised Learning Classification with multiple models.
Performed Linear Regression tasks on a specific dataset.
# Dataset (Magic Gamma Dataset)
Source : https://archive.ics.uci.edu/dataset/159/magic+gamma+telescope
The data are MC generated to simulate registration of high energy gamma particles in a ground-based atmospheric Cherenkov gamma telescope using the imaging technique.
    1.  fLength:  continuous  # major axis of ellipse [mm]
    2.  fWidth:   continuous  # minor axis of ellipse [mm] 
    3.  fSize:    continuous  # 10-log of sum of content of all pixels [in #phot]
    4.  fConc:    continuous  # ratio of sum of two highest pixels over fSize  [ratio]
    5.  fConc1:   continuous  # ratio of highest pixel over fSize  [ratio]
    6.  fAsym:    continuous  # distance from highest pixel to center, projected onto major axis [mm]
    7.  fM3Long:  continuous  # 3rd root of third moment along major axis  [mm] 
    8.  fM3Trans: continuous  # 3rd root of third moment along minor axis  [mm]
    9.  fAlpha:   continuous  # angle of major axis with vector to origin [deg]
   10.  fDist:    continuous  # distance from origin to center of ellipse [mm]
   11.  class:    g,h         # gamma (signal), hadron (background)

   g = gamma (signal):     12332
   h = hadron (background): 6688

#FLOW

1: One-hot encoding - changing the datatype of target variable
2: Visualization (Plotting histograms)
3: Training, Validation and Test datasets distribution.
4: kNN Implementation - Accuracy = 0.82
5: Naive Bayes - Accuracy = 0.73
6: Logistic Regression - Accuracy = 0.79
7: Support Vector Machine - Accuracy = 0.86
8: Plotting histograms between
  a) Loss vs Validation Loss
  b) Accuracy vs Validation accuracy
9: Neural Network
  a) Trained the model
    defined number of nodes - [16, 32, 64]
    defined dropout layer - [0 , 0.2]
    defined learning rate - [0.01, 0.005, 0.001]
    defined batch size - [32, 64, 128]
    defined epochs - 100
  b) Compiled the model using Optimizer Adam with loss (Binaric Crossentropy) and metrics (Accuracy)
  c) Finally assigned the validation loss with the least model loss if it is less then lest model loss
  d) Accuracy 
  

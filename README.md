# Technicals-CNN
Visually Predicting Stock Returns based on technicals using a CNN

#### ----- Notebook Overview: ----- ####
This Repository Contains the following three Notebooks:
1. TechniclaIndicatorsImplementation
Contains the algorithmic realization of the chosen technical indicators that are considered in the prediction algoorithm ()

List of considered technical indicators:
Relative Strength Index, Raw Volume, Boolinger Bands, Aroon, Price Volume Trend, Acceleration Bands, Stochastic, Chaikan Money Flow, Rate of Change, CCI, Keltner Channels, Exponential Moving Average, MACD, Money Flow Index, Ichimoku, William %R, Volume Min/Max

2. ImageTransformationPyplot:
Creation of the training and test dataset. This file transforms the daily returns as well as the resulting technicals into images as CNN input.

3. CNN_Implementation:
This file implements the Convolutional Neural Network, trains it using the created images and tests it against the test set of images.

#### ----- Directory Structure: ----- ####
Keras requietes the Input Data to be in the following directory structure:
Layer1: Notebooks
  Layer2: fullpriceinput.csv, y_train.csv, y_test.csv
    Layer3_A: RawStockData as dir of .txt files
    Layer3_B: Labelling
      Layer4_A: x_test
        Layer5_A: pos
        Layer5_B: neg
      Layer4_B: x_train
        Layer5_C: pos 
        Layer5_D: neg
        
#### ----- Required Python Libraries: ----- ####
pandas
numpy
ta
os
tqdm
matplotlib
pyts
mpl_toolkits.axes_grid1 
sklearn
tensorflow
keras
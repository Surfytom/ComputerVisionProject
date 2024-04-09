# Computer Vision Master Course Assignment

This repository contains all documents handed in for my computer vision assignment for my masters course in AI.

The main goal of the assignment was to train and evaluate different models on the MNIST dataset. Then use the best performing model to recognise digits from challenging images (and a video) which required general segmentation techniques to be used before a model was used to recognise the segmented digits

This repo contains 4 main files and 4 models. The models are a SVM (support vector machine), KNN (K-Nearest Neighbour), CNN (Convolutional Neural Network) and DNN (Deep Neural Network) all trained on the MNIST dataset.

## Files

### [ModelEvaluation.ipynb](https://github.com/Surfytom/ComputerVisionProject/blob/main/ModelEvaluation.ipynb)

This file contains all the evalutions for comparing the 4 models. 

There are confusion matrix's used to compare how each model handles recognising different numbers.

Images for the worst performing numbers are shown using matplotlib with a breif conclusion of why the model might not recognise those numbers correctly.

There is code showing how batch size testing was done using tensorboard.

### [SegmentationTesting.ipynb](https://github.com/Surfytom/ComputerVisionProject/blob/main/SegmentationTesting.ipynb)

This notebook shows the testing method used for the assignment. The best performing model from the evaluation notebook is used (CNN).

The assignment challenged us to segment 5 images and a video. These media got more challenging as they went on with image 1 being a simple black and white grid of numbers to the video being a person writing digits while moving the paper and casting shadows onto the digits.

The notebook contains comments and explanations for each segmentation step.

OutputVideo.avi shows an output for the final video with the segmentation method and model used for cropping and recognising the digits.

### [MLPWithMatrices.ipynb](https://github.com/Surfytom/ComputerVisionProject/blob/main/MLPWithMatrices.ipynb) and [SVMFromScratch.ipynb](https://github.com/Surfytom/ComputerVisionProject/blob/main/SVMFromScratch.ipynb)

These are both attempts at writing the logic for deep neural networks and svm from scratch using NumPy.

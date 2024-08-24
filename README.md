SCImageClassify Project
This repository contains a pipeline for preprocessing data, converting it into images, and performing basic image clustering analysis. The project then utilizes deep learning models to classify the images into different categories, focusing on cell classification.

Overview
The project is structured into several stages, each handled by different Jupyter notebooks:

Data Preprocessing (1-Data preprocessing.ipynb):
This notebook handles the initial data preprocessing, preparing the data for further analysis.

Matrix Clustering and Visualization (2-Matrix clustering and visualization.ipynb):
This stage involves clustering the data matrices and visualizing the results. It helps in identifying patterns and grouping similar data points.

Expression Matrix to Picture (3- Expression matrix to picture.ipynb):
The preprocessed data is transformed into images, making it suitable for image-based analysis and clustering.

Picture Unsupervised Clustering (4- Picture unsupervised clustering.ipynb):
This notebook performs unsupervised clustering on the images, providing an initial grouping of the data based on visual features.

Deep Learning Classification
After completing the preprocessing and clustering steps, the project moves on to image classification using deep learning models:

CNN Model (CNNModel.ipynb):
A Convolutional Neural Network (CNN) model is implemented to classify the images. This model is designed to capture the spatial hierarchies in the image data.

ResNet Model (model.ipynb):
The ResNet model is another deep learning architecture used in this project. It is particularly effective for image classification tasks due to its deep residual learning framework.

Training and Model Selection
The training process is managed in a dedicated training script. You can select between different models (e.g., CNN or ResNet) for the classification task. The models are trained to classify cell images, leveraging the preprocessed and clustered data from the earlier steps.

Requirements
This project requires the use of the pyDeepInsight library, which can be found at the following GitHub repository:

pyDeepInsight: https://github.com/alok-ai-lab/pyDeepInsight
pyDeepInsight is essential for converting high-dimensional data into images, which can then be used for deep learning-based classification. Follow the instructions in the pyDeepInsight repository to install and set up this library before running the notebooks in this project.

Usage
To run the project, follow these steps:

Start with the data preprocessing by running 1-Data preprocessing.ipynb.
Perform clustering and visualization with 2-Matrix clustering and visualization.ipynb.
Convert the expression matrices into images using 3- Expression matrix to picture.ipynb.
Apply unsupervised clustering on the images using 4- Picture unsupervised clustering.ipynb.
Choose and train a model by running either CNNModel.ipynb or model.ipynb.
Each notebook is self-contained and should be run in sequence to complete the full analysis and classification pipeline.

Conclusion
This repository provides a comprehensive approach to cell image classification, from preprocessing raw data to applying advanced deep learning models. The modular structure allows for flexibility in experimenting with different clustering techniques and classification models.

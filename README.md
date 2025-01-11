# Face Mask Detection using Convolutional Neural Network

This project implements a Convolutional Neural Network (CNN) to detect whether a person is wearing a face mask or not. It uses TensorFlow/Keras for model building and is designed to run on Google Colab.

## Features
- **Dataset Download**: Automatically downloads a face mask dataset from Kaggle.
- **Data Preprocessing**: Resizes images, converts them to numpy arrays, and scales pixel values.
- **Model Architecture**: A CNN with convolutional layers, pooling layers, and fully connected layers.
- **Training and Evaluation**: Trains the model on the dataset and evaluates it using accuracy and loss metrics.
- **Prediction System**: Allows predictions on custom input images.

## Installation and Setup
### Prerequisites
1. Python 3.7 or later.
2. Google Colab for running the script.
3. Kaggle API key (saved as `kaggle.json`).

### Steps to Run the Project
1. Upload your Kaggle API key (`kaggle.json`) to the Colab environment.
2. Run the script to set up the environment and download the dataset.
3. Follow the script to train the model and evaluate its performance.

## Dataset
The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/datasets/omkargurav/face-mask-dataset). It contains images of people with and without masks.

## Model Architecture
- **Convolutional Layers**: Extracts features from the input images.
- **MaxPooling Layers**: Reduces the spatial dimensions of the features.
- **Dropout Layers**: Prevents overfitting by randomly setting a fraction of input units to 0.
- **Fully Connected Layers**: Maps extracted features to output predictions.

## Results
- **Training Accuracy**: ~95%
- **Validation Accuracy**: ~90%
- Visualizations for training/validation accuracy and loss over epochs are generated.

## Usage
### Making Predictions
1. Provide the path to the image you want to predict.
2. The model outputs whether the person in the image is wearing a mask or not.

### Example:
```bash
Path of the image to be predicted: /content/sample_image.jpg
Prediction: Person is wearing a mask.
```


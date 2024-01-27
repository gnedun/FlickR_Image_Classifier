# FlickR_Image_Classifier

## Overview

Welcome to the "FlickR Image Classifier" project, a collaborative effort by Gokul Nedunsezhian, Jai Krishna Mounaguru, Rohit Madhu, and Rohan Pathak. This project focuses on building an image classifier that can identify and categorize various food items using a dataset obtained from FlickR.

## Problem Statement

The goal of this project is to develop a deep learning model capable of classifying images of different food items. Leveraging the FlickR API, we have gathered a substantial dataset consisting of 5000 images for each of the following food categories: burger, banana, apple, and pasta. The images were collected based on their interestingness, and the dataset serves as the foundation for training our image classification model.

## Data Collection

We utilized the FlickR API to search for the 5000 most interesting images in each food category and subsequently downloaded them for training our model. The process involved creating a subdirectory for each food item, specifying the number of images to download, and utilizing the API to fetch the images. The images were then stored in the designated directory for further processing.

## Model Building

### Data Preparation

The labels for each class were obtained from the training data directory, and image dimensions were set to 224x224 pixels. A data generator was set up using Keras to facilitate efficient loading and processing of the images during training.

### Transfer Learning

To build the image classification model, we employed transfer learning with the pre-trained Xception model. The base model, loaded with weights from the ImageNet dataset, had its layers frozen to prevent updates during training. The model architecture included global average pooling, dense layers, ReLU activation, dropout to prevent overfitting, and a final dense layer with softmax activation for the output classes.

### Model Training

The model was trained on the prepared dataset using categorical cross-entropy loss, the Adam optimizer, and accuracy as the evaluation metric. The training process was executed for a specified number of epochs, fine-tuning the model to recognize patterns in the food images.

## Model Deployment

The trained model was saved for future use and deployed for testing on a separate dataset. The model's accuracy was evaluated using test data, and a confusion matrix was generated to assess its performance across different food categories.

## Custom Image Testing

Additionally, the model was tested on a custom image downloaded from a Google search. The test image, representing an American burger from a local establishment, was preprocessed, and predictions were made. The results, including the top predicted food categories and their probabilities, were displayed in a tabular format.

## Conclusion

The "FlickR Image Classifier" project showcases the application of deep learning techniques to classify food images. The model, trained on a diverse dataset, demonstrates its ability to distinguish between different food items. This project is an exploration of image classification, transfer learning, and the practical application of machine learning in real-world scenarios.

Feel free to explore the code, try the model on your own images, and contribute to the project's development. If you have any questions or suggestions, don't hesitate to reach out to the project contributors. Happy coding!


Conclusion
The "FlickR Image Classifier" project showcases the application of deep learning techniques to classify food images. The model, trained on a diverse dataset, demonstrates its ability to distinguish between different food items. This project is an exploration of image classification, transfer learning, and the practical application of machine learning in real-world scenarios.

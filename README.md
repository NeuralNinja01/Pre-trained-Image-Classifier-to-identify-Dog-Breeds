# Pre-trained Image Classifier to identify Dog Breeds
### Overview

This project involves using three different pre-trained Convolutional Neural Networks (CNNs)—ResNet18, AlexNet, and VGG—to classify images of dogs and non-dogs. The task is to build an image classifier that first identifies whether the image contains a dog or not, and then if it is a dog, classifies the breed.

This project is part of the Udacity AI Programming with Python Nanodegree program with the AWS AI/ML Scholarship and focuses on evaluating and comparing the performance of the three pre-trained CNN models on a dog image dataset.

### Key Objectives

Objective 1: Identify whether an image contains a dog or not (classify as "dog" or "not-a-dog").

Objective 2: For images that contain a dog, classify the specific breed using one of the three pre-trained models: ResNet18, AlexNet, or VGG.

### Performance

VGG and AlexNet: Correctly identify "dog" and "not-a-dog" images 100% of the time.

VGG: Provides the best breed classification performance, identifying the correct breed over 90% of the time.

### Workflow Overview

The program performs the following tasks to achieve the objectives:

1. Timing the Program: The program runtime is measured using Python's time module to compute how long the program takes to classify all the images.

2. Input from the User: Command-line arguments are used to receive inputs from the user, such as the paths to the images and model choice.

3. Creating Pet Image Labels: Labels are generated based on the filenames of the pet images, which are then stored in a dictionary for easy lookup.

4. Classifying Images: Using the pre-trained CNN models (ResNet18, AlexNet, VGG), the images are classified into "dogs" and "not-dogs". The classifier’s predictions are compared against the pet image labels.

5. Classifying Labels as "Dogs" or "Not Dogs": The images are classified as "dogs" or "not dogs" using a reference file dognames.txt. This file contains the list of dog breed names used for comparison.

6. Results Calculation: The program calculates the accuracy of the classifier by comparing the classifier’s labels to the pet image labels, including the "is-a-dog" classification.

7. Printing Results: The final results are printed, displaying the accuracy for both the identification of dogs and the breed classification.

### Model Architectures Used

The project uses the following pre-trained models:

1. ResNet18: A deeper model known for its residual connections, making it effective for image classification tasks.

2. AlexNet: A classic model that introduced many important techniques in deep learning, such as the use of ReLU activation and dropout.

3. VGG: A model with a simple architecture of stacked convolutional layers, known for its depth and strong performance in image classification.

### Model Evaluation

Each model's performance is evaluated on the dataset using the two objectives:

Objective 1: Accuracy of identifying whether the image contains a dog.

Objective 2: Accuracy of classifying the breed of the dog, if applicable.

### Future Improvements:

1. Expanding the Dataset: The dataset could be expanded with more dog breeds or non-dog images for better evaluation.

2. Fine-tuning Models: Fine-tuning the pre-trained models on this specific dataset could improve classification accuracy.

3. Real-time Deployment: The model could be deployed to an application where users can upload images to classify dogs in real time.

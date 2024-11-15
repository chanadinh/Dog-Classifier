# Image Classification for a City Dog Show
## Overview
Image Classification for a City Dog Show project is a Python program that uses a pre-trained Convolutional Neural Network (CNN) model to classify pet images. The program compares the predicted classification against the actual breed (or type) of the pet based on the image filename and evaluates the performance of three different CNN models.

This project is useful for understanding image classification using transfer learning and comparing various CNN architectures for accuracy in classifying dog breeds.
## Project Description
Your city is hosting a citywide dog show, and you've volunteered to help with contestant registration. Participants are required to submit an image of their dog along with biographical information. However, some people might try to register pets that aren’t actual dogs.
## Features
- Image Classification: Classifies pet images using a selected pre-trained CNN model.
- Model Comparison: Compares the performance of three CNN models to determine the best one for dog breed classification.
- Evaluation Metrics: Calculates and displays the model’s accuracy and error rates for classification tasks, including whether an image is of a dog or not.
## Project Structure
- `check_images.py`: Main script that orchestrates the image classification, comparison, and evaluation process.
- `get_input_args.py`: Handles command-line arguments.
- `get_pet_labels.py`: Extracts the true label from each image filename.
- `classify_images.py`: Classifies each image using the selected CNN model.
- `adjust_results4_isadog.py`: Adjusts results to check if the classification is a dog or not.
- `calculates_results_stats.py`: Computes classification statistics.
- `print_results.py`: Displays results, including incorrect classifications.
## Prerequisites
1. Python 3.6+: This project requires Python 3.6 or higher.
2. PyTorch: Install PyTorch with support for your environment (CPU or GPU). Follow the instructions at PyTorch's installation page.
3. torchvision: This library provides popular datasets, model architectures, and image transformations for computer vision.
    ```bash
   pip install torchvision
    ```
5. PIL (Python Imaging Library): Pillow is required for image processing.
    ```bash
   pip install pillow
    ```
7. ImageNet Labels File: Download the imagenet1000_clsid_to_human.txt file. This file provides human-readable labels for the ImageNet classes and should be in the project directory.
8. Basic Python Skills: Understanding Python syntax, functions, and basic data handling is essential, as the focus is on using a provided classifier with Python.
## Usage
To classify images with the Dog Classifier, you can run two batch files depending on your environment:

1. Running run_models_batch.sh in Unix/Linux/OSX/Lab Workspace
- Open a terminal within the Project Workspace - Uploaded Images.
- Type the following command and hit enter: `run_models_batch.sh`
- This will execute check_images.py with all three model architectures on the images in the `pet_images` folder, saving the output files in the workspace.
2. Running run_models_batch_uploaded.sh in the Project Workspace (Uploaded Images)
- Open a terminal within the Project Workspace - Uploaded Images.
- Type the following command and hit enter: `sh run_models_batch_uploaded.sh`
- This will execute check_images.py with all three model architectures on the images in the `uploaded_images` folder, saving the output files in the workspace.

## Model Architectures
The project supports three CNN architectures:
- VGG: Deep CNN model known for accuracy in image recognition tasks.
- AlexNet: Efficient architecture with fewer parameters.
- ResNet: Residual network designed to address vanishing gradient problems.
## Output
1. Identifying which pet images are of dogs and which pet images aren't of dogs
2. Classifying the breeds of dogs, for the images that are of dogs
  
    ![alt text](https://video.udacity-data.com/topher/2018/March/5aa84e54_aipnd-intropythonlab-results/aipnd-intropythonlab-results.png)

## License
This project is open-source and available under the MIT License.

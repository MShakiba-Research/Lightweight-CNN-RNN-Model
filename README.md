# Lightweight CNN-RNN Model for Tomato Leaf Disease Detection

This repository contains the code and datasets for the research on a lightweight hybrid model combining Convolutional Neural Networks (CNN) and Recurrent Neural Networks (RNN) to detect tomato plant diseases from leaf images.

## Repository Structure

### 1. Augmented_Dataset
This folder includes the dataset that has been augmented using random rotation and brightness and contrast adjustment from the original dataset. The augmented data is used to improve the training process and model performance.

### 2. src
The `src` folder contains the source code for training and validating the models.

- **Training**: This subfolder contains the training code for five different models. The training scripts train the models for 50 epochs and save the model parameters into configuration files.
  
- **Validation**: This subfolder contains the validation code. The scripts load the models with trained parameter files from the `trained_model_parameters` folder and validate each model using the following metrics:
  - Confusion Matrix
  - Classification Report
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Inference Speed
  - Total Parameters
  - Memory Requirement
  - FLOPs value

### 3. trained_model_parameters
This folder contains the trained parameter files for the models. These files are used during the validation process to evaluate the models' performance.

### 4. ResultLog
The `ResultLog` folder contains CSV files storing the results of the five models. The results include metrics obtained from running the provided trained parameter files.

## Getting Started

### Prerequisites
Ensure you have the following software installed:
- Python 3.x
- Jupyter Notebook
- Required Python packages (see `requirements.txt`)

If you do not have Jupyter Notebook installed, you can set it up using Anaconda. Follow the instructions [here](https://docs.anaconda.com/anaconda/install/) to install Anaconda, which includes Jupyter Notebook.

### Installation
Clone the repository to your local machine:
```sh
git clone https://github.com/MShakiba-Research/Lightweight-CNN-RNN-Model.git
cd Lightweight-CNN-RNN-Model

### Setting Up the Environment
Create a virtual environment and install the required packages:
```sh
pip install -r requirements.txt

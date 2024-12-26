# AWS Deep Learning for Chicken Disease Classification

This repository demonstrates an end-to-end deep learning project designed to classify chicken diseases using convolutional neural networks (CNNs). The project leverages AWS services and is built to be scalable and efficient, suitable for both academic research and industrial application.

## Project Overview

The goal of this project is to utilize deep learning techniques to accurately classify various chicken diseases from images. This is crucial for improving poultry health management and can significantly impact the poultry industry by enabling early detection and treatment of diseases.

## Project Structure

- config/: Configuration files that manage model parameters, training settings, and environment variables.
- research/: Contains Jupyter notebooks used for trials and experimental setups. 
  - trials.ipynb: Notebook containing various experimental code snippets and trial models.
- src/CNN_Classifier/: Source code for the CNN model including utilities, configurations, and pipeline definitions. The structure is as follows:
  - components/: Modular components for the model such as data loaders, preprocessors, etc.
  - config/: Module configurations.
  - constants/: Definitions of constants used across the project.
  - entity/: Definitions of data entities and types.
  - pipeline/: End-to-end pipelines for training and prediction.
  - utils/: Utility functions and classes for logging, configurations, and other helper functions.
- .github/workflows/: Contains GitHub Actions workflows for continuous integration and deployment.

## Getting Started

### Prerequisites

- AWS Account
- Python 3.x
- Access to AWS services (S3, EC2, SageMaker, etc.)

### Installation

Clone this repository to your local machine:

```bash
git clone <repository-url>
cd AWS_DEEP_LEARNING_Chicken_disease_Classification-main
```

Install the necessary Python packages:

```bash
pip install -r requirements.txt
```

### Configuration

Before running the application, configure the necessary parameters in config/config.yaml. This includes setting up the AWS credentials, model parameters, and other necessary settings.

### Running the Project

To start training the model, run:

```bash
python src/CNN_Classifier/pipeline/train_pipeline.py
```

For predictions, execute:

```bash
python src/CNN_Classifier/pipeline/predict_pipeline.py
```


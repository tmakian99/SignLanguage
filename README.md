# Sign Language Recognition Program
Sign language in Real Time 
This is a program designed to recognize sign language signs using hand landmark data captured from a webcam. It utilizes the MediaPipe library for hand landmark detection and a RandomForestClassifier for machine learning-based sign recognition.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset Collection](#dataset-collection)
- [Data Annotation](#data-annotation)
- [Model Training](#model-training)
- [Inference](#inference)
- [License](#license)

## Introduction

This program captures hand landmark data through a webcam and uses machine learning to predict the corresponding sign language sign. It involves data collection, data annotation, model training, and real-time inference.

## Features

- Webcam-based data collection
- Data annotation with hand landmark coordinates
- Machine learning model training using RandomForestClassifier
- Real-time sign language recognition and display

## Requirements

- Python 3.x
- OpenCV (cv2)
- MediaPipe library
- Scikit-learn library
- TensorFlow (for padding sequences)

## Installation

1. Clone or download this repository to your local machine.
2. Install the required libraries using pip:


## Usage

1. Run the data collection script to collect images for each sign class.
2. Annotate the collected images by extracting hand landmark coordinates.
3. Train a RandomForestClassifier using the annotated data.
4. Run the inference script for real-time sign recognition.

## Dataset Collection

1. Run the data collection script (`data_collection.py`).
2. Capture images for each sign class by following the prompts.
3. Press the "Q" key to start capturing images.

## Data Annotation

1. Run the annotation script (`data_annotation.py`).
2. Extract hand landmark coordinates from collected images.
3. Save the processed data and labels as a pickle file.

## Model Training

1. Load the annotated data and labels from the pickle file.
2. Pad the data sequences to ensure consistent input sizes.
3. Split the data into training and testing sets.
4. Train a RandomForestClassifier using the training data.

## Inference

1. Run the inference script (`Final_Capstone.ipynb`).
2. Capture webcam frames and process hand landmark data.
3. Predict sign language signs in real-time.
4. Display predictions on the webcam feed.

## License

This project is licensed under the [MIT License](LICENSE).

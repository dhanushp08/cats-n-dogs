
# Dogs vs. Cats Image Classifier 

## Project Overview

This project implements a Convolutional Neural Network (CNN) using TensorFlow and Keras to classify images as either a "dog" or a "cat". It is a simple deep learning model which does the job of image classification.

## Features

  * **Image Classification:** Distinguishes between dog and cat images.
  * **CNN Architecture:** A custom-built CNN for image feature extraction.
  * **Data Handling:** Processes and normalizes image datasets.
  * **Model Training & Evaluation:** Trains the model and tracks its performance.
  * **Prediction:** Capable of classifying new, unseen images.

## Built With

  * **Python**
  * **TensorFlow & Keras**
  * **OpenCV (`cv2`)**
  * **Matplotlib**
  * **Kaggle API** (for dataset access)

## Dataset

The model is trained and validated on the **Dogs vs. Cats dataset** from Kaggle (provided by `salader`). This dataset includes a large collection of labeled images for both classes.

  * **Training Images:** 20,000
  * **Validation Images:** 5,000

## Model Architecture

The core of this project is a Convolutional Neural Network (CNN). It's designed with several convolutional layers (for feature detection) followed by pooling layers (for downsampling). The network concludes with dense (fully connected) layers and uses dropout for regularization to prevent overfitting.

## Performance

After 6 training epochs, the model achieved approximately:

  * **Training Accuracy:** `~89.03%`
  * **Validation Accuracy:** `~80.80%`

## How to Run 

This project is designed to be run in a **Jupyter Notebook** environment, such as **Google Colab**.

1.  **Get the Code:**

      * Clone this repository: `git clone https://github.com/dhanushp08/cats-n-dogs.git`
      * Navigate into the project directory: `cd cats-n-dogs`

2.  **Kaggle API Key:**

      * You'll need a `kaggle.json` file (your API credentials) to download the dataset. Generate this from your Kaggle account settings.
      * Place `kaggle.json` in the appropriate location for your environment (e.g., `~/.kaggle/` for local Jupyter, or upload it to Google Colab when prompted).

3.  **Run the Notebook:**

      * Open `bclassification.ipynb` in your Jupyter/Colab environment.
      * Execute all cells. The notebook will handle:
          * Dataset download and extraction.
          * Data preparation and normalization.
          * CNN model construction and training.
          * Saving the trained model (`my_model.h5`).
          * Demonstrating a prediction on a sample image.

## Sample Prediction

To show how the model works, we tested it with pictures of a dog and a cat.

**1. Testing with a Dog:**

  * **Input Image:**
    ( If you put your `dog.jpg` image here)

  * **Model's Answer:**

    ```
    [[1]]
    ```

  * **What it Means:** The model gave `1`, meaning it correctly saw a **dog**.

**2. Testing with a Cat:**

  * **Input Image:**
    ( If you put your `cat.jpg` image here)

  * **Model's Answer:**

    ```
    [[0]]
    ```

  * **What it Means:** The model gave `0`, meaning it correctly saw a **cat**.

-----

##  How the project can be enhanced in near future

  * **Data Augmentation:** Increase dataset diversity to improve robustness.
  * **Transfer Learning:** Experiment with pre-trained models (e.g., VGG16, ResNet) for potentially higher accuracy.
  * **Hyperparameter Tuning:** Optimize model parameters for better performance.
  * **Deployment:** Explore deploying the model (e.g., web app, mobile app).

-----

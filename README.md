# Colorizing Black and White Videos using Convolutional Autoencoder (CAE)

This repository contains code and instructions for colorizing black and white videos using Convolutional Autoencoder (CAE). The CAE leverages deep learning techniques to transform grayscale videos into colorized versions, bringing them to life with vibrant and realistic colors.

## Dataset

To perform the video colorization, you will need a dataset of black and white videos. The dataset can be obtained from various sources or created using your own videos. Ensure that the videos are in grayscale format for accurate colorization.

## Implementation

### Data Preparation

1. **Step 1**: Dataset Loading and Preprocessing
   - Load the black and white video dataset.
   - Preprocess the video frames, such as resizing, normalizing, and converting to grayscale.

2. **Step 2**: Data Augmentation (Optional)
   - Apply data augmentation techniques, such as random cropping, flipping, or rotation, to increase the diversity of the training data.

### Convolutional Autoencoder (CAE)

The CAE implementation includes the following steps:

1. **Step 1**: Model Architecture
   - Build the CAE model using TensorFlow and Keras.
   - The encoder part of the CAE extracts features from the grayscale frames, while the decoder part generates the corresponding colorized frames.

2. **Step 2**: Training
   - Compile the CAE model with appropriate optimizer and loss function.
   - Train the CAE model on the black and white video dataset.

3. **Step 3**: Inference
   - Take black and white video frames and pass them through the trained CAE model for colorization.
   - Visualize and display the original grayscale frames and their corresponding colorized frames.

### Colorizing Video Frames

To colorize video frames using the trained CAE model, follow these steps:

1. **Step 1**: Load Video Frames
   - Provide the path to the black and white video.
   - Capture the video frames using OpenCV.
   - Preprocess the frames by resizing them to a specific size, e.g., 224x224.

2. **Step 2**: Colorize Frames
   - Pass the preprocessed grayscale frames through the trained CAE model.
   - Obtain the colorized frames as the model's output.

3. **Step 3**: Display Results
   - Visualize and display the original grayscale frames alongside their colorized versions.
   - Optionally, save the colorized video frames to create a colorized video output.

## Requirements

- Python 3.x
- TensorFlow
- Keras
- OpenCV
- NumPy
- Matplotlib

Please make sure to install the required dependencies before running the code.

## Usage

1. Clone the repository to your local machine.
2. Prepare the black and white video dataset and place it in the appropriate directory.
3. Modify the code to specify the dataset path and other necessary parameters.
4. Run the code to train the CAE model and perform video colorization.
5. Observe the colorized video frames and evaluate the results.
6. Customize the code as needed for your specific use case.

Feel free to experiment with different model architectures, hyperparameters, and preprocessing techniques to improve the colorization performance.

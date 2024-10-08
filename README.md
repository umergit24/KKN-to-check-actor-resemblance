## K-Nearest Neighbors Celebrity Look-Alike

This code implements a k-nearest neighbors algorithm to find the celebrity that a given input image most resembles. It uses a dataset of celebrity images and their corresponding labels, and calculates the Euclidean distance between the input image and each image in the dataset. The closest matches are then returned as the potential look-alikes.

### Inputs

*   **`dataset`:** Path to the .mat file containing the celebrity image dataset and labels (e.g., `/content/drive/My Drive/ML/data.mat`).
*   **`test_image`:** Path to the input image to be compared against the dataset (e.g., `/content/drive/My Drive/ML/notme.png`).

### Outputs

*   **1-NN:** The celebrity from the dataset whose image is closest to the input image based on Euclidean distance.
*   **3-NN:** The three celebrities from the dataset whose images are closest to the input image based on Euclidean distance.
*   **5-NN:** The five celebrities from the dataset whose images are closest to the input image based on Euclidean distance.

### Usage

1.  **Upload `data.mat` to Google Drive.** This file contains the celebrity images and their corresponding labels.
2.  **Specify the paths to `dataset` and `test_image` in the code.** Replace the placeholder paths with the actual paths to your files.
3.  **Run the code.** The outputs will show the celebrity look-alikes based on 1-NN, 3-NN, and 5-NN. 

### Notes

*   The code is designed to run in Google Colab.
*   The input image should be resized to 32x32 pixels and reshaped to a 1D array before being compared to the dataset.
*   You can adjust the value of `k` in the `for` loops to change the number of nearest neighbors considered. 

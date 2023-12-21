# Brain Tumor Segmentation

This repository contains code for a project that uses the U-Net architecture to segment brain tumors from MRI scans. The project involves downloading a dataset, preprocessing the images, and training a U-Net model.

## Setup

1. Clone the repository.
2. Install dependencies with pip:
```
pip install -r requirements.txt
```
3. Run the main script:
```
python main.py
```

## Code Overview

The code in this repository does the following:

1. Downloads and unzips a dataset of brain tumor MRI scans from figshare.
2. Loads the data into numpy arrays.
3. Preprocesses the images by resizing them, normalizing them, and creating masks for the tumors.
4. Splits the data into training, validation, and test sets.
5. Defines a U-Net model for image segmentation.
6. Trains the model on the training data, using dice coefficient as a metric and saving the best model parameters.
7. Evaluates the trained model on test data.

## Dependencies

This project uses Google Colab's environment and requires these Python libraries:

- numpy
- hdf5storage
- cv2
- matplotlib.pyplot
- keras
- tensorflow
- sklearn

## Data

The brain tumor dataset used in this project can be found [here](https://figshare.com/articles/dataset/brain_tumor_dataset/1512427).

## Results

The results of this project include saved .npy files of processed images and masks, as well as saved models in .h5 format.

For more details about each step of this project, please refer to comments in the code.

## Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the terms of the MIT license.

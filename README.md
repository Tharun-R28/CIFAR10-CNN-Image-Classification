# CIFAR-10 Image Classification using CNN

A deep learning project that classifies images from the CIFAR-10 dataset using a custom Convolutional Neural Network (CNN) built with PyTorch.

## Project Overview

Image classification is a computer vision task in which a model learns to identify objects from images. In this project, a CNN is trained on the CIFAR-10 dataset to classify images into one of ten categories.

The project covers dataset loading, image preprocessing, CNN architecture design, model training, and test accuracy evaluation.

## Dataset

The CIFAR-10 dataset contains 60,000 colour images of size 32 × 32 pixels across 10 classes.

The dataset consists of:
- 50,000 training images
- 10,000 test images

**Classes:** Airplane, Automobile, Bird, Cat, Deer, Dog, Frog, Horse, Ship, and Truck.

The dataset is downloaded automatically by `torchvision.datasets.CIFAR10`.

## Technologies Used

- Python
- PyTorch
- Torchvision
- Convolutional Neural Networks (CNN)
- Jupyter Notebook

## Model Architecture

The CNN contains three convolutional blocks, each using:
- Convolutional layers
- ReLU activation
- Max pooling

The extracted features are flattened and passed through fully connected layers to produce predictions for the ten classes.

## Data Preprocessing

The images are converted into tensors and normalized using a mean and standard deviation of 0.5 for each RGB channel.

## Training Configuration

| Parameter | Value |
|---|---|
| Batch size | 64 |
| Epochs | 10 |
| Optimizer | Adam |
| Loss function | Cross-Entropy Loss |
| Framework | PyTorch |

## Model Evaluation

The trained model is evaluated on the CIFAR-10 test dataset. Test accuracy is calculated by comparing predicted labels with the actual labels.

The measured accuracy can be found in the notebook output after running the evaluation cell.

## Project Structure

```text
CIFAR10-CNN-Image-Classification/
├── CNN_for_CIFAR10.ipynb
├── README.md
└── .gitignore
```

The dataset is downloaded into the `data/` directory when the notebook runs and is not included in the repository.

## How to Run

1. Clone this repository.
2. Install the required libraries.
3. Open the notebook in Jupyter Notebook or JupyterLab.
4. Run the notebook cells in order.

### Installation

```bash
pip install torch torchvision matplotlib jupyter
```

### Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/CIFAR10-CNN-Image-Classification.git
```

Replace `YOUR-USERNAME` with your GitHub username.

### Launch JupyterLab

```bash
cd CIFAR10-CNN-Image-Classification
jupyter lab
```

Open `CNN_for_CIFAR10.ipynb` and run the cells. The dataset will be downloaded automatically.

## Learning Outcomes

- Understanding CNN architecture and feature extraction
- Applying image normalization
- Training a neural network using backpropagation
- Using PyTorch DataLoaders
- Evaluating a classifier using test accuracy

## Future Improvements

- Add validation data and validation accuracy
- Display a confusion matrix and per-class precision and recall
- Plot training loss and accuracy curves
- Experiment with data augmentation and hyperparameter tuning

## Author

Tharun R

GitHub:  https://github.com/Tharun-R28

---

This project was developed for learning and practising deep learning and computer vision with PyTorch.
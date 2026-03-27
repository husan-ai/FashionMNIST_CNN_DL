# Fashion MNIST CNN Classifier (PyTorch)

This project implements a **Convolutional Neural Network (CNN)** using PyTorch to classify clothing images from the **FashionMNIST dataset**.

---

## Project Overview

The goal of this project is to build a simple deep learning model that can classify grayscale images of clothing into 10 categories such as:

* T-shirt/top
* Trouser
* Pullover
* Dress
* Coat
* Sandal
* Shirt
* Sneaker
* Bag
* Ankle boot

---

## Technologies Used

* Python
* PyTorch
* Torchvision
* Jupyter Notebook

---

## Dataset

We used the **FashionMNIST dataset** provided by `torchvision.datasets`.

* Training samples: 60,000
* Test samples: 10,000
* Image size: 28x28 (grayscale)

---

## Model Architecture

The CNN model (`KiyimCNN`) consists of:

* Conv2d (1 → 8 channels)
* ReLU activation
* MaxPooling (2x2)
* Flatten layer
* Fully Connected layers:

  * 1568 → 128
  * 128 → 10 (output classes)

Input feature calculation:
28x28 → Conv → 28x28 → Pool → 14x14
8 × 14 × 14 = 1568

---

## Training Details

* Loss Function: `CrossEntropyLoss`
* Optimizer: `Adam`
* Learning Rate: `0.002`
* Epochs: `5`
* Batch size: `32`

---

## Results

After training, the model achieves approximately:

**Accuracy: ~85% – 90%** (depends on run)

---

## How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/fashion-mnist-cnn-pytorch.git
```

2. Install dependencies:

```bash
pip install torch torchvision
```

3. Run the notebook:

```bash
jupyter notebook
```

---

## Key Learnings

* Understanding CNN basics
* Working with PyTorch datasets and DataLoader
* Building custom models using `nn.Module`
* Training and evaluating deep learning models

---

## Author

Husan


---

## Future Improvements

* Add more Conv layers
* Use Dropout for regularization
* Increase epochs
* Achieve 90%+ accuracy

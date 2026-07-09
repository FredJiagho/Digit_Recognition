# Digit Recognition

This repository contains deep learning experiments for digit recognition using PyTorch. It includes models and training utilities for both single-digit MNIST classification and a custom two-digit recognition task.

## Repository Structure

- `part2-mnist/` - Single-digit MNIST classification experiments
  - `nnet_fc.py` - Fully connected neural network model for MNIST
  - `nnet_cnn.py` - Convolutional neural network model for MNIST
  - `train_utils.py` - Training and evaluation helpers for MNIST models
  - `mnist_model_fully_connected.pt` - Example trained model weights

- `part2-twodigit/` - Two-digit recognition experiments
  - `mlp.py` - Multi-layer perceptron model for the two-digit problem
  - `conv.py` - Convolutional model for the two-digit problem
  - `train_utils.py` - Training and evaluation helpers for the two-digit models
  - `utils_multiMNIST.py` - Dataset utilities for generating and loading two-digit images
  - `sample_images/` - Example generated two-digit images
  - `mnist_model_fully_connected.pt` - Example trained model weights

- `Datasets/` - Project dataset storage (dataset files may be stored here)
- `utils.py` - Shared utility functions for the repository
- `requirements.txt` - Python package dependencies

## Installation

1. Create and activate a Python virtual environment:

   ```bash
   python -m venv venv
   .\venv\Scripts\activate
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Usage

### MNIST single-digit training

Run the training script from `part2-mnist` to train or evaluate MNIST models. For example:

```bash
python part2-mnist\train_utils.py
```

### Two-digit recognition training

Run the training script from `part2-twodigit` to train or evaluate models on the two-digit dataset. For example:

```bash
python part2-twodigit\train_utils.py
```

## Notes

- The repository is designed for experiments with digit recognition models.
- Pretrained model weights are included for demonstration purposes.
- The two-digit dataset is generated using utilities in `part2-twodigit/utils_multiMNIST.py`.

## License

This repository is provided for educational and research purposes.

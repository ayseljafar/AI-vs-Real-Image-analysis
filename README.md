# AI vs Real Image Analysis

This project implements a deep learning model to distinguish between AI-generated artwork and real artwork using Convolutional Neural Networks (CNN). The analysis provides insights into the visual characteristics that differentiate AI-generated art from human-created art.

## Project Overview

The project uses a CNN model trained on a dataset of AI-generated artwork and real artwork to classify images into these two categories. The model employs various data augmentation techniques and early stopping to prevent overfitting.

## Features

- Image classification between AI-generated and real artwork
- Data augmentation for improved model generalization
- CNN architecture with multiple convolutional layers
- Early stopping mechanism to prevent overfitting
- Visualization of training and validation metrics
- Support for various image dimensions

## Requirements

- Python 3.x
- TensorFlow
- OpenCV
- NumPy
- Pandas
- Matplotlib
- Pillow

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/AI-vs-Real-Image-analysiss.git
cd AI-vs-Real-Image-analysiss
```

2. Install the required packages:
```bash
pip install -r requirements.txt
```

## Project Structure

```
AI-vs-Real-Image-analysiss/
├── images/                 # Directory containing sample images
├── AIvsRealAArt.ipynb     # Jupyter notebook with analysis
├── aivsrealimageanalysis.py  # Main Python script
└── README.md              # Project documentation
```

## Usage

1. Prepare your dataset:
   - Place AI-generated artwork in the `AiArtData` directory
   - Place real artwork in the `RealArt` directory

2. Run the analysis:
```bash
python aivsrealimageanalysis.py
```

## Model Architecture

The CNN model consists of:
- Three convolutional layers with ReLU activation
- MaxPooling layers after each convolutional layer
- Flatten layer
- Dense layer with 512 units and ReLU activation
- Dropout layer (0.5)
- Output layer with softmax activation

## Training Process

The model is trained with the following specifications:
- Image size: 255x255 pixels
- Batch size: 64 for training, 16 for validation
- Optimizer: Adam with learning rate 0.001
- Early stopping with patience of 20 epochs
- Data augmentation including rotation, width/height shifts, shear, zoom, and horizontal flips

## Results

The model provides:
- Training and validation accuracy metrics
- Training and validation loss curves
- Classification performance on test data

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Dataset contributors
- TensorFlow team for the deep learning framework
- OpenCV team for image processing capabilities

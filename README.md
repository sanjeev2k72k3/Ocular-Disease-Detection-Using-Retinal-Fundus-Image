# Ocular Disease Detection Project

This project implements a deep learning-based system for detecting ocular diseases from fundus images. It combines advanced image processing techniques with a state-of-the-art deep learning architecture to achieve high accuracy in disease classification.

## Overview

The project focuses on the detection and classification of ocular diseases using fundus images. It employs a sophisticated image processing pipeline followed by a hybrid deep learning architecture to achieve accurate disease classification.

## Features

- Advanced image processing pipeline for Retinal Fundus Images.
- Custom Attention U-Net architecture combined with DenseNet201
- Data augmentation techniques for improved model generalization
- Comprehensive evaluation metrics and visualization tools
- Support for multiple ocular disease classifications
- Real-time image processing capabilities
- Automated disease detection and classification

## Project Structure

```
├── Image Procesing Pipeline.ipynb    # Image preprocessing and enhancement
├── Model Training.ipynb              # Deep learning model training
├── requirements.txt                  # Project dependencies
└── Image Processsing Steps.png       # Visualization of processing steps
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ocular-project.git
cd ocular-project
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

## Methodology

### Image Processing Pipeline

The `Image Procesing Pipeline.ipynb` implements a comprehensive image processing pipeline that includes:

1. **Color Enhancement**
   - RGB to HSV conversion
   - Adaptive histogram equalization
   - Color balance adjustment

2. **Green Channel Extraction**
   - Optimal channel selection
   - Contrast enhancement
   - Noise reduction

3. **Illumination Correction**
   - CLAHE (Contrast Limited Adaptive Histogram Equalization)
   - Background normalization
   - Shadow removal

4. **Noise Reduction**
   - Bilateral filtering
   - Gaussian smoothing
   - Edge preservation

5. **Edge Enhancement**
   - Sobel edge detection
   - Laplacian filtering
   - Edge sharpening

6. **Field of View Standardization**
   - Circular mask creation
   - Boundary detection
   - Region of interest extraction

7. **Resolution Standardization**
   - Image resizing
   - Aspect ratio preservation
   - Quality maintenance

### Model Architecture

The `Model Training.ipynb` implements a hybrid deep learning architecture:

1. **Backbone Network (DenseNet201)**
   - Pre-trained on ImageNet
   - Feature extraction capabilities
   - Transfer learning approach

2. **Attention U-Net**
   - Custom attention mechanism
   - Skip connections
   - Multi-scale feature extraction

3. **Ensemble Approach**
   - Feature concatenation
   - Dense layers for classification
   - Dropout for regularization

## Training Process

1. **Data Augmentation**
   - Rotation
   - Scaling
   - Flipping
   - Brightness adjustment
   - Contrast variation

2. **Model Training**
   - Batch size: 32
   - Learning rate: 0.000015
   - Optimizer: AdamW
   - Loss function: Categorical Cross-entropy
   - Early stopping implementation

3. **Evaluation Metrics**
   - Accuracy
   - Precision
   - Recall
   - F1-score
   - ROC-AUC

## Results

The model achieves high accuracy of 98.3% in disease classification with:
- Robust feature extraction
- Effective disease detection
- Real-time processing capabilities
- High generalization ability

## Requirements

- Python 3.7+
- TensorFlow 2.8.0+
- OpenCV 4.5.1+
- Other dependencies listed in requirements.txt

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The project uses DenseNet201 pre-trained on ImageNet
- Thanks to all contributors and the open-source community
- Special thanks to the medical imaging community for their valuable resources 

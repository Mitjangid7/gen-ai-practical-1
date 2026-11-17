# Practical No. 01: Image Classification using CNN and Transfer Learning

## Student Information

- **Name:** Mit Jangid
- **PRN:** 202401110072
- **Batch:** A1
- **Subject:** Generative AI

## Aim

To implement image classification using a Convolutional Neural Network (CNN) trained from scratch and compare its performance with transfer learning using MobileNetV2 pre-trained on ImageNet.

## Dataset

This project uses the **Fashion-MNIST** dataset, containing 30,000 balanced images from five selected categories:

1. T-shirt/top
2. Trouser
3. Pullover
4. Sneaker
5. Bag

Each category contains 6,000 images.

| Dataset Split | Number of Images |
|---|---:|
| Training | 24,000 |
| Validation | 3,000 |
| Testing | 3,000 |
| **Total** | **30,000** |

The original images are grayscale and have a resolution of 28 × 28 pixels. For MobileNetV2, images are converted to three channels and resized to 96 × 96 pixels.

## Models Implemented

### 1. CNN from Scratch
- Convolutional layers for feature extraction.
- Batch normalization and max pooling.
- Dropout for regularization.
- Softmax output layer for five-class classification.

### 2. MobileNetV2 Transfer Learning
- Uses MobileNetV2 pre-trained on ImageNet.
- Initial feature extraction with frozen base-model layers.
- Fine-tuning of the final MobileNetV2 layers.
- Five-class softmax classification output.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Google Colab

## Evaluation

Both models are evaluated using the same held-out test dataset. Evaluation includes:

- Accuracy
- Weighted Precision
- Weighted Recall
- Weighted F1-score
- Classification Report
- Confusion Matrix
- Training and Validation Accuracy/Loss Curves

## Experimental Results

| Model | Test Accuracy |
|---|---:|
| CNN from Scratch | 98.20% |
| MobileNetV2 Transfer Learning | 97.53% |

The results are obtained from the executed notebook.

## Repository Contents

- `Mit_Jangid_Fashion_Transfer_Learning.ipynb` – Complete implementation with code and outputs.
- `README.md` – Project overview and documentation.

## Conclusion

A CNN trained from scratch and a MobileNetV2 transfer-learning model were implemented for Fashion-MNIST image classification. Both models achieved strong classification performance. Their performance was compared using test accuracy, precision, recall, F1-score, classification reports, confusion matrices and training curves.

## Author

**Mit Jangid**  
TY AIML | Batch A1

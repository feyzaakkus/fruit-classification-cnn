# Fruit Classification Using CNN

## Project Description

This project implements a deep learning-based image classification system using a Convolutional Neural Network (CNN). The model classifies fruit images into five categories: Apple, Banana, Orange, Pear, and Strawberry.

## Dataset

- **Dataset:** Fruits-360 (Original Size)
- **Source:** [Kaggle – Fruits-360](https://www.kaggle.com/datasets/moltean/fruits)
- **Selected Classes:** Apple 10, Banana 2, Orange 2, Pear 1, Strawberry 2
- **Total Images:** 3,166

| Dataset Split | Number of Images |
|---|---:|
| Training | 1,586 |
| Validation | 794 |
| Test | 786 |

## Model Architecture

A custom CNN model was developed using PyTorch.

The model includes:
- Three convolutional layers with 32, 64, and 128 filters
- Batch Normalization
- ReLU activation
- Max Pooling
- Adaptive Average Pooling
- Dropout (0.3)
- Fully connected output layer with 5 classes

**Total Parameters:** 94,341

## Training Configuration

| Parameter | Value |
|---|---|
| Input Size | 100 × 100 × 3 |
| Epochs | 15 |
| Batch Size | 32 |
| Learning Rate | 0.001 |
| Optimizer | Adam |
| Loss Function | Weighted CrossEntropyLoss |
| Dropout | 0.3 |

## Results

| Metric | Result |
|---|---:|
| Validation Accuracy | 100% |
| Test Accuracy | 100% |
| Macro Precision | 100% |
| Macro Recall | 100% |
| Macro F1-Score | 100% |
| Training Time | 109.30 seconds |
| Inference Time | 0.538 ms |

## Real-World Image Testing

The model was also tested using five fruit photographs taken with a mobile phone.

- Correct Predictions: 2 out of 5
- Real-World Accuracy: 40%

The difference between dataset performance and real-world performance may be related to variations in lighting, background, camera angle, and image conditions.

## Deployment

The trained model was deployed using Gradio. Users can upload fruit images and view the model's predicted class probabilities.

## Technologies Used

- Python
- PyTorch
- Torchvision
- Google Colab
- Gradio
- Scikit-learn
- Matplotlib

## Repository Contents

- `Fruit_Classification_CNN.ipynb`: Model development, training, evaluation, and deployment notebook.

## Author

Computer Engineering Student Project

# BreakTheCaptcha
# CAPTCHA Generation, Classification, and OCR

## Overview
This project implements a system for CAPTCHA generation, classification, and optical character recognition (OCR). The codebase includes scripts for generating CAPTCHA images with different difficulty levels, training a CNN for classification, and implementing a CRNN for OCR.

## Directory Structure
- Task 0 \ -- Captcha Generator\
         -- Dataset Generator
- Task 1 \ -- Classification Model \
         -- Confusion Matrix and Evaluation
- Task 2 \ -- OCR Dataset Generator
         -- CRNN Model \
         -- Training the Model
         
## Running in Google Colab
This project was implemented in **Google Colab**. To run it:
1. **Upload necessary font files** to **Google Drive**.
2. **Mount Google Drive** in Colab:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')

## Installation and Dependency Libraries
- Python 3.7+
- OpenCV
- Pillow
- NLTK
- PyTorch
- Torchvision
- scikit-learn
- matplotlib
- seaborn

Already Imported in Colab so no need for external downloads.

## Approach
CAPTCHA Generation: Uses OpenCV and PIL to generate CAPTCHA images with easy, hard, and bonus variations. The bonus dataset is generated but not fully utilized in the OCR task.

Classification: Implements a CNN with two convolutional layers, max pooling, and two fully connected layers to classify CAPTCHA images into 100 word classes. Experiments were conducted with various learning rates and batch sizes.

OCR: Implements a CRNN with CTC loss for extracting text from CAPTCHA images. An advanced decoding function was attempted but could not be completed due to time constraints.

## Task Update

### Completed:

CAPTCHA Generation (easy, hard, and bonus datasets)

CAPTCHA Classification (CNN model trained and evaluated)

OCR (CRNN with CTC loss implemented and evaluated)

### Incomplete:

Bonus OCR Task (bonus OCR not completed)

## Evaluation Metrics

Classification Task: Accuracy, Precision, Recall, F1-score, Confusion Matrix.

OCR Task: CTC Loss, Loss Curve Over Epochs, Predicted vs Actual Text.




# Oxford-IIIT-Pet-BREED-CLASSIFICATION
Problem Statement  This project focuses on image classification using the Oxford-IIIT Pet Dataset. The goal is to predict the breed of a cat or dog from a photo. This is a multi-class classification task with 37 pet breeds. 
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1HvVuajTCe2kQs3PI5Qbe86OMnKCEdDpN?authuser=1#scrollTo=n_Iskzdi487F)
## Project Structure

- `01_baseline.ipynb` — simple baseline model
- `02_resnet18_transfer_learning.ipynb` — transfer learning with ResNet18
- `images/` — saved plots and visualizations

## Dataset

The project uses the Oxford-IIIT Pet Dataset from torchvision.

The dataset contains images of 37 pet breeds.

## Approach

### Day 1: Baseline

A simple baseline model was trained to establish an initial performance level.

### Day 2: Transfer Learning

A pretrained ResNet18 model was used.

Training was done in two stages:

1. Freeze pretrained layers and train only the final classifier.
2. Unfreeze the top ResNet block and fine-tune it with a lower learning rate.

## Results

The transfer learning model achieved:

- Test Accuracy: **87.8%**
- Macro F1-score: **0.88**
- Weighted F1-score: **0.88**

## Visualizations

### Training Loss

![Loss Curve](images/loss_curve.png)

### Training Accuracy

![Accuracy Curve](images/accuracy_curve.png)

### Confusion Matrix

![Confusion Matrix](images/confusion_matrix.png)

## Conclusion

Transfer learning with ResNet18 significantly improved performance compared to the simple baseline.

The model performs well overall, but still makes mistakes on visually similar pet breeds.

Further improvements could include stronger augmentation, additional fine-tu

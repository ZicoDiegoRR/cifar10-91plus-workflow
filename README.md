# CIFAR-10 Custom CNN Architecture with 91+% Test Accuracy

A complete PyTorch workflow for CIFAR-10 image classification, reaching over 91% test accuracy with a fully custom convolutional neural network — no pretrained architectures like ResNet or VGG. This project demonstrates building, training, and evaluating deep CNNs from scratch, highlighting best practices for data preprocessing, regularization, and optimization. 

---

## 📌 Features 

✅ Custom-built CNN architecture (no transfer learning)
✅ Data normalization and augmentation
✅ Dropout and Batch Normalization
✅ Learning rate scheduling with `ReduceLROnPlateau`
✅ Early stopping to prevent overfitting
✅ High test accuracy (~91.6%) with ~19 million parameters
✅ Clear training curves visualization
✅ Fully reproducible training and evaluation scripts

---

## 🗂️ Dataset

This project uses the CIFAR-10 dataset, consisting of 60,000 32x32 RGB images in 10 classes, with 50,000 images for training and 10,000 for testing.

---

🚀 Model Architecture

The architecture consists of:
- 9 convolutional layers with increasing feature maps (32 → 1024)
- Interleaved `BatchNorm2d` and `ReLU` activations
- `AdaptiveAvgPool2d` to handle spatial size reduction
- Fully connected classifier with `Dropout` for regularization
- Total parameters: 19.5 million

---

## 🛠️ Training Details

Optimizer              : `SGD` with `momentum` and `weight_decay`
Learning rate scheduler: `ReduceLROnPlateau` (monitors test loss)
Loss function          : `CrossEntropyLoss`
Data augmentation      : Random cropping and horizontal flipping
Early stopping         : Stops training when test loss stops improving

---

## 🖥️ How to Run

No manual installation is needed. Just run the notebook and you're ready to go.

---

## 📊 Visualization

This project produces training and test loss curves, along with test accuracy plots using `matplotlib`.

---

## 📖 License

MIT License — feel free to use, modify, and share!

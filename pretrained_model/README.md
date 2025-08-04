# 91.61% Test Accuracy

This model was trained previously with the current workflow.
Here's the description:
- Epoch                   = 84
- Optimizer               = `SGD` (with `momentum`)
- Learning rate           = 0.01
- Learning rate scheduler = `ReduceLROnPlateau`
- Parameters count        = 19,525,706
- Batch size              = 128
- Weight decay            = 0.000001
- Data augmentation       = `RandomCrop` and `RandomHorizontalFlip`
- GPU used                = T4
- Training time           = 1h 20m (100 epochs)
- Loss function           = `CrossEntropyLoss`

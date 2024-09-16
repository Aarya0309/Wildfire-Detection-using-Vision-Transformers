# Final Models Used for Wildfire Detection

This document provides the links to the pre-trained models used in the final version of the wildfire detection code. The models are stored on Kaggle and can be accessed directly.

### 1. **Binary ViT Model (10 Epochs)**

- **Purpose:** Used to classify images as either **Fire** or **No Fire**.
- **Model:** Vision Transformer pre-trained for binary classification.
- **Link to Model:** [Binary ViT 10 Epochs](https://www.kaggle.com/datasets/aaryamahajanpabha/capstone-models?select=Binary_VIT_10epochs)

### 2. **Fire Subclass ViT Model**

- **Purpose:** Used to classify images that contain fire into specific subclasses:
  - Smoke from fires
  - Both smoke and fire
- **Model:** Vision Transformer fine-tuned for fire subclass classification.
- **Link to Model:** [Fire Subclass Model](https://www.kaggle.com/datasets/aaryamahajanpabha/capstone-models?select=fire_subclass_model_VIT)

### 3. **No-Fire Subclass ViT Model (10 Epochs)**

- **Purpose:** Used to classify no-fire images into the following subclasses:
  - Forested areas without confounding elements
  - Fire confounding elements
  - Smoke confounding elements
- **Model:** Vision Transformer fine-tuned for no-fire subclass classification.
- **Link to Model:** [No-Fire Subclass Model (10 Epochs)](https://www.kaggle.com/datasets/aaryamahajanpabha/capstone-models?select=nofire_subclass_model_VIT_10epochs)

### How to Use the Models

In the provided demo code, these models are loaded using the following lines:
```python
binary_model = ViTForImageClassification.from_pretrained('/kaggle/input/capstone-models/Binary_VIT_10epochs/Binary_VIT_10epochs')
fire_subclass_model = ViTForImageClassification.from_pretrained('/kaggle/input/capstone-models/fire_subclass_model_VIT/fire_subclass_model_VIT')
nofire_subclass_model = ViTForImageClassification.from_pretrained('/kaggle/input/10epochs-nofiremodel/nofire_subclass_model_VIT_10epochs')
```
This file will provide clarity to anyone running the project, ensuring they can access the exact models required for execution.

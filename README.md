# Wildfire-Detection-using-Vision-Transformers

This project explores the use of Vision Transformers (ViTs) for early wildfire detection through image classification. The cascading ViT model employed in this project improves the accuracy of fire and no-fire classification using multiple dedicated submodels.

## Project Overview

Wildfires pose a significant risk to ecosystems and human life, and early detection is crucial for effective intervention. This project leverages the power of Vision Transformers (ViT) for wildfire image classification with the following goals:
- Binary classification of images into **Fire** and **No-Fire**.
- Subclassification of both fire and no-fire images into more specific categories (e.g., smoke, fire, shadows).

### Key Features
- **Binary ViT Classifier**: Classifies images into fire or no-fire with an accuracy of 97.8%.
- **Cascading Submodels**: Dedicated ViT models further classify fire and no-fire subclasses, achieving an overall accuracy of 88.54%.
- **Attention Visualization**: Heatmaps highlight the regions of images that contributed to model predictions, aiding in interpretability.

## Dataset
The dataset consists of 2700 aerial and ground-based images categorized into **fire** and **no-fire** classes. It includes multiple fire scenarios, including smoke, flames, and confounding elements like shadows.

## Results
The model achieved the following metrics:
- **Binary ViT Accuracy**: 97.8%
- **Cascading Model Accuracy**: 88.54%
- **Comparison with Dual-Dataset DL**: Outperformed existing models in accuracy and precision.

## How to Run the Project
1. Clone this repository:
    ```bash
    git clone https://github.com/yourusername/Wildfire-Detection-ViTs.git
    ```
2. Install dependencies:
    ```bash
    pip install transformers torch
    ```
3. Run the notebooks in the `notebooks/` folder to see the code and results.

## Future Work
- **Hyperparameter tuning** for further performance improvement.
- **Transfer learning** to enhance model robustness on larger datasets.
- **Explainability** improvements through more detailed attention maps.

## Acknowledgments
This project is inspired by various research papers exploring the potential of Vision Transformers for image classification tasks.

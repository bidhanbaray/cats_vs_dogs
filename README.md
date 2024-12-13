# cats_vs_dogs
This work was done as homework for the course ECSE 6410: Pattern Recognition at UGA in Fall 2024. 

This homework aims to develop a Machine Learning (ML) model to automatically classify cats or dogs given any image containing either of those two. The task involves training various classifiers using publicly available datasets, incorporating effective pre-processing and feature extraction techniques to ensure the model performs well on unseen data.

## Project Structure

### Objective
- Develop a Machine Learning (ML) model to classify images of cats and dogs.
- Focus on effective preprocessing, feature extraction, and model evaluation.

### Summary
- Used Kaggle Cats-vs-Dogs dataset (25,000 images) and CIFAR-10 dataset for external testing.
- Images were resized and normalized with techniques like CLAHE, Sobel, and AHE.
- Features extracted included HOG, LBP, and Color Histograms.
- Multiple classifiers were trained and evaluated, including SVM, Random Forest, and MLP.
- Final model achieved 77% accuracy using SVC with 5-fold cross-validation.

### Datasets
- **Kaggle Cats-vs-Dogs**: 25,000 images equally split between cats and dogs.
- **CIFAR-10**: 10,000 images of cats and dogs used for external testing.

### Preprocessing
- Resized images to 32x32 for efficiency.
- Applied photogrammetric normalization techniques (CLAHE, Sobel, etc.).
- Explored both RGB and grayscale formats.

### Feature Extraction
- Extracted features:
  - Histogram of Oriented Gradients (HOG)
  - Local Binary Pattern (LBP)
  - Color Histograms
- Combined features for enhanced performance.

### Experimental Setup
- Tested classifiers with various feature combinations:
  - Random Forest
  - SVM
  - XGBoost
  - MLP
- Ensemble models and PCA were employed for optimization.

### Results
- Best Accuracy:
  - 77% with SVM on Kaggle Cats-vs-Dogs dataset.
  - 64% on CIFAR-10 dataset for external testing.
- Feature combination of LBP + HOG yielded optimal results.

## Key Findings
- Preprocessing techniques had limited impact on improving performance.
- Smaller image resolutions (32x32) performed comparably to larger sizes.
- Combination of gradient, texture, and color features enhanced classification.


### Acknowledgements
- Kaggle Cats-vs-Dogs Dataset: [Link](https://www.kaggle.com/c/dogs-vs-cats)
- CIFAR-10 Dataset: [Link](https://www.cs.toronto.edu/~kriz/cifar.html)

# Advanced Classification using Machine Learning in Healthcare

## Introduction
X-rays are widely used in medical practice to identify various diseases. However, diagnoses often depend on a doctor's experience, which can lead to improper treatment. Modern artificial intelligence and pattern recognition methods enable the creation of expert systems that can establish diagnoses automatically.

This project demonstrates how to upload images, transform them, and determine the key features for disease classification.

Two approaches to image (disease) classification are explored:
1. Classical machine learning methods and their comparison
2. Convolutional Neural Networks (CNNs)

## Materials and Methods
The project consists of four stages:
1. Downloading and preprocessing images
2. Extracting image features
3. Comparing classical classification methods
4. Building and training a Convolutional Neural Network

The dataset used is [Kaggle's COVID-19 Image Dataset](https://www.kaggle.com/datasets/pranavraikokte/covid19-image-dataset), licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

## Prerequisites
The following tools and libraries are required:

- [Python](https://www.python.org/)
- [`os`](https://docs.python.org/3/library/os.html)
- [`numpy`](https://numpy.org/)
- [`glob`](https://docs.python.org/3/library/glob.html)
- [`seaborn`](https://seaborn.pydata.org/)
- [`matplotlib`](https://matplotlib.org/)
- [`mahotas`](https://mahotas.readthedocs.io/)
- [`keras`](https://keras.io/)
- [`scikit-learn`](https://scikit-learn.org/)
- [`pandas`](https://pandas.pydata.org/)

## Project Structure

### Data Preprocessing
- Images are resized to 224×224 pixels.
- RGB/RGBA images are converted to grayscale.
- Pixel values are normalized to the [0,1] range.

### Feature Extraction
- Haralick texture features are extracted using `mahotas`.
- Features are scaled using `StandardScaler`.

### Classical Machine Learning Models
The following models are implemented and compared:
- Logistic Regression
- K-Nearest Neighbors
- Linear SVM
- RBF SVM
- Gaussian Process
- Decision Tree
- Random Forest
- Multi-layer Perceptron
- AdaBoost
- Naive Bayes
- Quadratic Discriminant Analysis

### Convolutional Neural Network (CNN)
- Three convolutional layers with max-pooling and ReLU activation
- Dropout for regularization
- Dense layers for classification
- Trained with data augmentation (rotation, zoom, shifts, flips)

## Results
The project provides:
- Comparative analysis of classical ML models
- Visual representation of training and testing accuracy
- Confusion matrices for model evaluation
- Detailed classification reports
- A diagnostic function for processing new X-ray images

The CNN achieves higher accuracy than classical methods, albeit with longer training times.

## Usage
To diagnose a new X-ray image using the trained CNN model:
```python
result = diagnosis("path/to/xray/image.jpg")
print(f"Final diagnosis: {result}")
```

This function:
1. Loads and preprocesses the image.
2. Makes a prediction using the trained model.
3. Visualizes the confidence levels.
4. Returns the predicted diagnosis (`Covid`, `Normal`, or `Viral Pneumonia`).

## Conclusion
This project demonstrates how to create an expert system for diagnosing diseases based on X-ray images. The principles used can be applied to any type of X-ray analysis, not just COVID diagnostics.

Through this work, we explored image processing techniques, feature extraction methods, and various classification approaches, comparing traditional machine learning with deep learning solutions.
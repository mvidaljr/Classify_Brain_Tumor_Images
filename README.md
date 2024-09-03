# Brain Tumor Image Classification

## Project Overview

This project involves building a Convolutional Neural Network (CNN) using TensorFlow to classify brain MRI images into categories such as tumor or no tumor. The goal is to develop an accurate and efficient model that can assist in the early detection and diagnosis of brain tumors, potentially improving patient outcomes.

## Dataset

- **Source:** The dataset consists of labeled MRI images of the brain, with each image categorized as either having a tumor or being tumor-free.
- **Classes:** The primary classes include `Tumor` and `No Tumor`.

## Tools & Libraries Used

- **Data Handling:**
  - `TensorFlow` and `Keras` for building and training the CNN model.
  - `Pandas` for data manipulation and preprocessing.
- **Image Processing:**
  - `OpenCV` or `PIL` for image loading, resizing, and preprocessing.
- **Model Evaluation:**
  - Metrics such as accuracy, precision, recall, and AUC (Area Under the Curve) to evaluate model performance.

## Methodology

### Data Preprocessing:

- **Image Resizing:**
  - All images were resized to a consistent dimension to ensure uniform input for the CNN.
  
- **Data Augmentation:**
  - Applied augmentation techniques like rotation, zoom, and horizontal flipping to increase the diversity of the training set and improve the model's robustness.

### Model Development:

- **CNN Architecture:**
  - Designed a deep Convolutional Neural Network with multiple layers of convolution, pooling, and fully connected layers to capture complex features from the MRI images.
  - Used ReLU as the activation function for hidden layers and softmax for the output layer.
  
- **Model Training:**
  - Trained the CNN using categorical cross-entropy loss and optimized the model with the Adam optimizer.
  - Techniques such as dropout and batch normalization were employed to prevent overfitting and improve generalization.

### Model Evaluation:

- **Confusion Matrix:**
  - Analyzed the confusion matrix to evaluate the model’s performance across the different classes.
  
- **ROC Curve:**
  - Generated ROC curves to assess the model's ability to distinguish between tumor and no-tumor cases.

- **Example Usage:**
  ```python
  predictions = model.predict(new_image)
  ```

## Results

The CNN model demonstrated high accuracy in classifying brain MRI images, making it a valuable tool for assisting radiologists and medical professionals in the early detection of brain tumors.

## Conclusion

This project highlights the potential of deep learning in medical imaging, particularly in the classification of brain tumors. The model's performance indicates that CNNs can be effectively used to support medical diagnoses, potentially improving patient outcomes through earlier detection.

## Future Work

- Explore transfer learning techniques to enhance model performance using pre-trained networks.
- Expand the model to classify other types of brain anomalies and integrate it into a clinical decision support system.
- Experiment with more advanced architectures like 3D CNNs to capture spatial information in the MRI scans.


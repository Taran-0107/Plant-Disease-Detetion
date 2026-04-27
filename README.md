# Plant Disease Detection using Convolutional Neural Networks

## Abstract
This project presents a deep learning-based approach for plant disease detection using leaf images. A Convolutional Neural Network (CNN) is trained on a dataset comprising 38 disease classes to enable accurate and early identification of plant diseases. The system aims to support precision agriculture and improve crop health monitoring.

---

## Problem Statement
Plant diseases significantly affect agricultural productivity and food security. Manual identification is time-consuming and prone to error. This project addresses the need for an automated, accurate, and scalable solution using deep learning techniques.

---

## Dataset
- Total Training Images: 70,295  
- Total Validation Images: 17,572  
- Number of Classes: 38  
- Image Size: 128 x 120  
- Source: Kaggle Plant Disease Dataset  

---

## Methodology

### Data Preprocessing
- Image resizing to standard dimensions  
- Conversion to RGB format  
- Batch processing using Keras (batch size = 32)  

### Model Architecture
The CNN architecture consists of five convolutional blocks followed by fully connected layers:

- Convolutional Layers:
  - Filters: 32, 64, 128, 256, 512  
  - Kernel Size: 3x3  
  - Activation: ReLU  
  - Max Pooling: 2x2  

- Fully Connected Layers:
  - Flatten layer  
  - Dense layers (~1400 neurons)  
  - Output layer with 38 neurons (Softmax activation)  

### Training Configuration
- Optimizer: Adam  
- Learning Rate: 0.0001  
- Loss Function: Categorical Crossentropy  
- Epochs: 10  

---

## Results

- Training Accuracy: ~97%  
- Validation Accuracy: ~95%  

The model demonstrates strong performance across multiple plant species and disease categories. Evaluation metrics such as precision, recall, and F1-score indicate consistent classification quality across most classes.

---

## Evaluation

Performance was assessed using:
- Accuracy  
- Precision  
- Recall  
- F1-score  

The model shows good generalization with minimal overfitting.

---

## Sample Prediction

The trained model successfully predicts plant diseases from unseen leaf images. Example output includes classification of diseases such as *Apple Cedar Apple Rust* with high confidence.

---

## Applications

- Automated crop disease detection  
- Precision agriculture systems  
- Decision support tools for farmers  
- Agricultural research and monitoring  

---

## Limitations

- Performance depends on image quality  
- Limited to trained disease classes  
- Requires computational resources for training  

---

## Future Work

- Integration with transfer learning models (e.g., ResNet, EfficientNet)  
- Deployment as a web or mobile application  
- Real-time disease detection  
- Expansion of dataset to include more crops and conditions  

---

## Technology Stack

- Python  
- TensorFlow / Keras  
- NumPy, Pandas  
- Matplotlib, Seaborn  

---

## Authors

- Roshan Kumar Mahto  
- Tarandeep Singh  

---

## References

- https://www.tensorflow.org/  
- https://www.tensorflow.org/guide/keras  
- https://www.kaggle.com/datasets/vipoooool/new-plant-diseases-dataset  
- https://seaborn.pydata.org/  
- https://ieeexplore.ieee.org/document/8437085  

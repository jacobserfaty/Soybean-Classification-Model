# Soybean Seed CNN Classification Model

### Introduction
"Good seed is the foundation of good crops." - Norman Borlaug

Welcome to the Soybean Seed CNN Classification Model project! This project focuses on improving the efficiency of agricultural tech businesses by enhancing the quality of soybean seeds. High-quality soybean seeds have the potential to result in increased crop yield, resist common soybean diseases and pests, and possess desirable genetic traits like tolerance to specific environmental conditions. This README provides an overview of the project, its goals, data, modeling, business recommendations, and potential model improvements.

### Business Understanding
Our goal is to enhance agricultural tech businesses by improving the quality of the soybean seeds they use. To achieve this, we aim to:

- Collect soybean seed images from agricultural tech businesses in the soybean market to use in a classification model.
- Create a model that can distinguish between viable and non-viable seeds.
- Integrate this model into agricultural hardware for sorting seeds efficiently.

### Data Understanding
The dataset consists of 5513 images of soybean seeds with the following characteristics:

- The data is equally balanced.
- Each image is 227x227 pixels.
- There are 5 classes:
    - Intact
    - Broken
    - Immature
    - Skin-damaged
    - Spotted

![class_dist](https://github.com/jacobserfaty/Soybean-Classification-Model/blob/main/images/class_dist.png)

### Modeling
For this project, all models used are Convolutional Neural Networks (CNNs). 

The base model layout consists of:
- 3 2D-convolutional layers.
- 3 max-pooling layers.
- 1 hidden layer.

![confusion1](https://github.com/jacobserfaty/Soybean-Classification-Model/blob/main/images/confusion1.png)

The final model layout includes:
- 3 2D-convolutional layers.
- 3 max-pooling layers.
- 3 hidden layers.
- 2 dropout layers.
- Bias, padding, and L2 regularization.

![confusion4](https://github.com/jacobserfaty/Soybean-Classification-Model/blob/main/images/confusion4.png)

### Business Recommendations
Based on our findings, here are the key business recommendations:

- The recommended model for soybean seed identification is the final classification model.
- Integrate this model into a seed-sorting mechanism that can classify each seed in real-time.
- The model would benefit from higher-quality color images.
- Ensure that the dataset is free from mislabeled data.

![seeds](https://github.com/jacobserfaty/Soybean-Classification-Model/blob/main/images/seeds.png)

### Model Improvements
To enhance the model further, consider the following improvements:

- Implement transfer learning models trained specifically for seed identification.
- Address misclassification by comparing classes and considering a binary classification model.
  
Thank you for your interest in the Soybean Seed CNN Classification Model project. For more details and to access the code and dataset, please refer to the project repository.

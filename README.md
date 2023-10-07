# Sri Lanka Institute of Information Technology

## Breast Cancer Classification Using Deep Learning Architectures

### Deep Learning - SE4050

### Group Assignment Report

📚 **IT Number and Names:**

- IT20611774 - G.G.R Sachintha
- IT20189112 - Silva W. S. J
- IT20653668 - Dilshi G. A
- IT20107000 - Priyangani K. A. V

## Introduction 📖

Breast cancer is a major global health concern for women, characterized by the uncontrollable growth of abnormal breast cells, often forming tumors. Early detection is crucial for timely intervention and better outcomes. Deep learning, especially Convolutional Neural Networks (CNNs), can enhance breast cancer diagnosis accuracy and efficiency.

🔬 **Algorithms Used**:

CNNs are ideal for image analysis. In breast cancer classification, CNNs analyze mammograms, histopathological slides, or medical images to distinguish benign from malignant breast tissues. Key CNN components include convolutional layers, pooling layers, activation functions (ReLU, Sigmoid), and an output layer with an appropriate activation function.

This assignment employs three custom CNN models with distinct architectures. Additionally, transfer learning with MobileNet is utilized to leverage pre-trained models, saving time and resources.

## Dataset and Data Analysis 📊

**Dataset Description**:

- Histopathology images of Invasive Ductal Carcinoma (IDC) - the most common breast cancer subtype.
- Captured from whole mount slide images of Breast Cancer (BCa) specimens at 40x magnification.
- Dataset aims to assign aggressiveness grades to breast cancer samples, focusing on IDC identification.
- Contains 277,524 image patches of size 50x50, with 198,738 IDC-negative and 78,786 IDC-positive samples.

**Data Preprocessing Techniques**:

1. Data Balancing (20000 images each for benign and malignant).
2. Resizing and Standardization.
3. Normalization and Rescaling (1./255).
4. Data Augmentation (random rotation, flipping, zooming).
5. Data Cleaning (removing duplicates).
6. Shuffling.

These techniques ensure quality, uniformity, and diversity in the dataset, improving model performance.

## Model Architecture 🧠

**IT20611774 Model**:

- 12 layers: 1 Data Pre-processing, 4 Convolutional, 4 MaxPooling, 1 Flatten, and 2 Fully Connected (Dense) layers.
- ReLU activation function.
- Output layer with sigmoid activation for binary classification.

**IT20189112 Model**:

- 11 layers: 4 Convolutional, 4 MaxPooling, 2 Fully Connected (Dense), and 1 Flatten layer.
- ReLU activation function in convolutional layers.
- Softmax activation in the output layer for classification.

**IT20653668 Model**:

- 3 Convolutional Layers with MaxPooling.
- Dropout Layer (0.2 dropout rate).
- Flatten Layer.
- 2 Fully Connected (Dense) Layers.

**IT20107000 Model**:

- 1 Convolutional Layer.
- Max Pooling Layer.
- Flatten Layer.
- 2 Dense Layers with ReLU activation.
- Softmax activation in the output layer.

## Results and Comparison 📊

**Model Performance Metrics**:

- Model 1:

  - Accuracy: 87.95%
  - Precision: 87.74%
  - Recall: 87.56%
  - F1-score: 87.65%

- Model 2:

  - Accuracy: 87.95%
  - Precision: 75.00%
  - Recall: 77.00%
  - F1-score: 76.00%

- Model 3:

  - Accuracy: 87.49%
  - Precision: 87.99%
  - Recall: 91.76%
  - F1-score: 89.84%

- Model 4:
  - Accuracy: 91.00%
  - Precision: 91.37%
  - Recall: 90.52%
  - F1-score: 90.95%

**Conclusion** 📝

- MobileNet transfer learning (Model 4) performed best.
- Model 3 balances precision and recall effectively.
- Model 1 offers competitive accuracy and precision.
- Model 2 shows promise but needs improvement, especially in precision and recall.

Deep learning models hold promise for breast cancer classification but require continuous refinement for optimal performance.

## References 📚

- [PubMed: Breast Cancer Classification](https://www.ncbi.nlm.nih.gov/pubmed/27563488)
- [Kaggle: Breast Cancer Histopathology Images Dataset](https://www.kaggle.com/datasets)
- [Deep Learning Series](https://www.analyticsvidhya.com/blog/2020/10/what-is-the-convolutional-neural-network-architecture/)
- [Deep Learning in Medical Imaging](http://spie.org/Publications/Proceedings/Paper/10.1117/12.2043872)

## Thanks for reading! 🙌🏼

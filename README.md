# CSC 219 Project 2: Time Series Forecasting using LSTM and CNN

## Project Overview:
In this collaborative project, our team embarks on a two-fold exploration of time series data. We endeavor to tackle both classification and regression tasks using advanced deep learning techniques, specifically Long Short-Term Memory (LSTM) and Convolutional Neural Networks (CNN). These methodologies will be applied to distinguish real strawberries from imposters in one part of the project and predict energy consumption within a low-energy building in the other.

## Part 1: Strawberry Authentication

### Dataset Highlights:
  Training Dataset: 613 samples.
  Testing Dataset: 370 samples.
  Dataset Length: 235 data points.
  Data Dimensionality: One-dimensional.
  Classes:
    Class 1: Authentic Strawberries
    Class 2: Non-Strawberry Counterparts (including adulterated strawberries and other fruits).

### Workflow:

1. Data Preprocessing: We initiate with data acquisition and preprocessing, which involves cleaning, normalizing, and splitting the data into training and testing sets.

2. Feature Extraction: Relevant features are extracted from FTIR spectroscopy data, using techniques like spectral analysis, peak detection, and statistical moments.

3. Classification Models:
  Basic classifiers (e.g., logistic regression, random forest) are built to establish performance baselines.
  Deep learning models like CNN and LSTM are explored for one-dimensional data, enhancing the ability to capture complex patterns.

4. Model Evaluation: Model performance is assessed using metrics such as accuracy, precision, recall, and F1-score for both training and testing datasets.

5. Hyperparameter Tuning: Model parameters and architecture are fine-tuned for optimal performance, including adjusting learning rates, batch sizes, and activation functions.

6. Cross-Validation: K-fold cross-validation ensures robustness and prevents overfitting.

7. Model Interpretability: Beyond classification, we explore model interpretability techniques like feature importance analysis and gradient-based approaches.

## Part 2: Energy Consumption Forecasting

### Dataset Description:
The dataset comprises 19,735 instances and 29 real feature types.
It spans approximately 4.5 months with observations recorded at 10-minute intervals, focusing on energy consumption within a low-energy building.

### Workflow:

1. Data Preprocessing: Data quality and consistency are ensured by handling null and duplicate values, and unnecessary columns (date and target variable) are dropped.

2. LSTM Model for Regression:
    Long Short-Term Memory (LSTM) models are employed for time series regression.
    Model design, training, and monitoring are executed to prevent overfitting.
    Model performance is evaluated using Mean Squared Error (MSE) and Root Mean Squared Error (RMSE) metrics.

3. Optimizing Sequence Length (N) for LSTM Model: The impact of sequence length (N) on pattern capture is investigated.

4. Enhanced LSTM Model: Bidirectional and Attention layers are added to improve the LSTM model's performance.

5. CNN Model for Regression:
  Convolutional Neural Networks (CNN) are applied to regression tasks on time series data.
  Data preprocessing, model design, training, and evaluation are performed similar to LSTM.

4. Optimizing Sequence Length (N) for CNN Model: Efficient sequence length (N) is determined for the CNN model.

By seamlessly blending classification and regression tasks, our project aims to showcase the versatility of deep learning techniques like LSTM and CNN in handling a wide array of time series data challenges. Whether discerning the authenticity of strawberries or forecasting energy consumption, our journey promises to offer valuable insights and practical models for these real-world applications.

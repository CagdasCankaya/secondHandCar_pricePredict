#  Used Car Price Prediction – A Regression Problem
This project presents a regression model developed to predict the prices of used cars based on various vehicle features. The model was built and trained using TensorFlow and Keras.

All numerical features were normalized using TensorFlow's Normalization layer to ensure faster and more stable learning. The artificial neural network (ANN) consists of:

# Input Layer
# 3 Hidden Layers (128 neurons each, ReLU activation)
# 1 Output Layer (predicts the car price)

The model outputs a continuous value representing the estimated car price. The loss function used is Mean Absolute Error (MAE) and the evaluation metric is Root Mean Squared Error (RMSE).

To increase efficiency, TensorFlow’s tf.data pipeline was used for data loading and batching. Visualizations were performed with matplotlib.

#  Libraries Used
TensorFlow / Keras

Pandas

NumPy

Seaborn & Matplotlib

Scikit-learn

#  PROJECT STEPS

# 1- Data Preparation
Loaded and cleaned data from CSV file.

# 2- Normalization
Applied normalization to numerical columns via Keras layer.

# 3- Model Architecture
Input → 3 Hidden Layers → Output (ANN model)

# 4- Training
Optimizer: Adam, Loss: MAE, Metric: RMSE

# 5- Evaluation
Loss and RMSE plots, comparison of predictions vs true values.


# File Structure
├── train.csv          # Used car dataset
├── model.png          # Model architecture image
├── scripts/           # Code for training and evaluation
├── README.md          # Project documentation
└── requirements.txt   # Required libraries

# Suggestions for Improvement
Try deeper or more advanced architectures

Include categorical variables like brand, city

Use ensemble or transfer learning techniques

# Product Owner 
Çağdaş ÇANKAYA

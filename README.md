
# 🩺 Breast Cancer Diagnosis Predictor


### 📊 Overview

The Breast Cancer Diagnosis Predictor is an application built using machine learning techniques to assist medical professionals in diagnosing breast cancer. The app takes in several measurements of breast masses and predicts whether they are benign or malignant. It provides a visual representation of the data through a radar chart and also displays the probability of the mass being benign or malignant. The app is designed to help streamline the process of diagnosing breast cancer based on scientific data.

The app was developed as an educational exercise using the Breast Cancer Wisconsin (Diagnostic) Data Set. Please note that the dataset and the app are intended solely for educational purposes and should not be used in clinical environments.

### ✨ Features
  - Data Visualization: Display a radar chart with three categories of data: mean, standard error, and worst-case measurements for each attribute.
  - Prediction: Use a machine learning model (Logistic Regression) to predict whether a given set of measurements corresponds to a benign or malignant mass.
  - Probability Display: Show the probabilities for both benign and malignant predictions.
  - Interactive Sidebar: Allows the user to manually adjust the measurements for prediction.

### 🛠️ Installation

To set up this application, you can directly install the dependencies using pip. Follow these steps:


```bash
  git clone <repository_url>
```
Navigate to the project directory:

```bash
  cd <project_directory>
```
Install the required dependencies: It is recommended to use a virtual environment, but if you prefer not to, you can directly install the dependencies using pip:

```bash
  pip install -r requirements.txt
```
This will install all necessary packages, including numpy, pandas, pickle5, plotly, scikit_learn, and streamlit.

Run the application: After the dependencies are installed, you can start the app by running:

```bash
  streamlit run app/main.py
```

This will open the app in your default web browser. You can now input the measurements through the sidebar, and the app will provide the predicted diagnosis and a radar chart.

### 🧑‍💻 Model Creation

The model is based on Logistic Regression. It uses the Breast Cancer dataset and performs the following steps:

- Data Preprocessing: Cleans the dataset by removing irrelevant columns and encoding the diagnosis (benign or malignant) as binary values.
- Data Scaling: The features are scaled using StandardScaler for better model performance.
- Model Training: The data is split into training and testing sets, and the Logistic Regression model is trained on the training data.
- Model Evaluation: The accuracy and classification report are generated to evaluate the model's performance.

### 🌐 Streamlit Application

The Streamlit application allows the user to input cell measurements through a sidebar. These inputs are processed and displayed using a radar chart, and predictions are shown based on the trained Logistic Regression model.

### 📁 File Structure

The app's files are structured as follows:

- app/main.py: Main script for the Streamlit application.
- app/assets/style.css: Custom CSS file to style the application.
- model/model.pkl: Pickled Logistic Regression model.
- model/scaler.pkl: Pickled StandardScaler for data scaling.



### 📜License

[MIT](https://choosealicense.com/licenses/mit/)


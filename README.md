#  Heart Disease Prediction

This project is a **machine learning model** that predicts whether a person has heart disease based on medical attributes. It uses a **Logistic Regression classifier** trained on a dataset of patient health records.



##  Project Overview

* **Goal**: Predict heart disease (1 = Defective Heart, 0 = Healthy Heart).
* **Dataset**: A CSV file (`data.csv`) containing medical records such as age, sex, blood pressure, cholesterol, heart rate, etc.
* **Model Used**: Logistic Regression.
* **Evaluation Metric**: Accuracy Score on training and testing datasets.



## Project Structure


heart_disease_prediction.py   # Main Python script
data.csv                      # Dataset (should be placed in /content/ for Colab or same folder for local run)
README.md                     # Project documentation



##  Dependencies

Make sure you have the following libraries installed:

  bash
pip install numpy pandas scikit-learn




##  How to Run

1. Clone this repository or download the project files.
2. Place the dataset (`data.csv`) in the correct path (`/content/` if using Google Colab, or same directory if local).
3. Run the script:

   bash
   python heart_disease_prediction.py
   
4. The script will:

   * Load and preprocess the dataset.
   * Split the data into training and test sets.
   * Train a Logistic Regression model.
   * Print accuracy on training and test data.
   * Run a **sample prediction** for given input data.



## Sample Output


Accuracy on Training data :  0.85
Accuracy on Test data :  0.81
The Person has Heart Disease



##  Example Prediction

Input data format (tuple of values):


(age, sex, cp, trestbps, chol, fbs, restecg, thalach, exang, oldpeak, slope, ca, thal)


Example:

python
input_data = (62,0,0,140,268,0,0,160,0,3.6,0,2,2)


Prediction Output:

* `0` → Person does **not** have heart disease.
* `1` → Person **has** heart disease

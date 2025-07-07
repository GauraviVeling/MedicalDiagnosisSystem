# Medical Diagnosis System

Medical Diagnosis System is a web-based machine learning application that predicts diseases based on user-input symptoms using the Random Forest algorithm. It includes a data collection tool to improve model accuracy and also explores Naive Bayes for comparison during development.

## Features

- Predicts diseases based on 132 symptoms
- Supports 41 possible disease classifications
- Trained using a Random Forest model on 4920 samples
- Includes a data collection tool (`survey.csv`) for model retraining
- User-friendly web interface built with Flask
  
## Dataset Source
This project uses a publicly available dataset with 132 symptoms and 41 diseases (4920 samples).
Download it from Kaggle:
[🔗 Disease Symptom Description Dataset on Kaggle](https://www.kaggle.com/datasets/itachi9604/disease-symptom-description-dataset?select=dataset.csv)

## Machine Learning Models Used

- Random Forest — main algorithm used for prediction
- Naive Bayes — used for experimentation and comparison

## Tech Stack

- Python
- Flask (web framework)
- HTML and CSS (frontend)
- Scikit-learn, Pandas, NumPy (for machine learning and data processing)

## How to Run the Application

1. **Clone the repository**
2. **Install dependencies**
   pip install flask scikit-learn pandas numpy
3. **Start the Flask application**
   python app.py
4. **Open your browser and go to**
   http://localhost:5000
   
## Output Example

Users can select symptoms via checkboxes on the website. Based on the selected symptoms, the trained machine learning model (Random Forest) analyzes the input and predicts the most probable disease in real-time.

### Data Collection (Survey Tool)

The system also includes a data collection feature where users who have been officially diagnosed with a disease can fill out their symptoms and select their confirmed disease. This data is saved to the `survey.csv` file.
You can later use this collected data to:
- Expand your dataset
- Preprocess and combine it with the existing data
- Retrain the model for improved accuracy

This feedback loop allows the model to evolve and improve over time based on real-world user input.

**Medic AI: Disease Prediction and Medicine Recommendation System with Machine Learning**

This project is a Disease Prediction and Medicine Recommendation System that uses machine learning to help users understand and manage their health. By analyzing user-input symptoms, the system predicts possible diseases and provides detailed recommendations including precautions, medications, workouts, and dietary advice.


**🚀 Features**

1. User Friendly Interface

An intuitive and clean interface that allows users to enter symptoms easily. The system supports autocomplete suggestions for faster and more accurate inputs.

2. Machine Learning Disease Prediction

Our application uses a trained machine learning model to predict possible diseases based on user provided symptoms. The predictions are accurate and optimized with real medical symptom data.

3. Personalized Medical Recommendations

For every predicted disease, the system provides:

Top medicines

Prescription guidance

Helpful precautions

Recommended diet

Workout suggestions

These recommendations are tailored to support better health management.

4. Flask Web Application

The entire system runs on a lightweight Flask backend, making it fast, reliable, and easy to deploy on any platform, including:

Local machine

Cloud servers

Hosting services like Render, Heroku, or Railway

5. Privacy and Security

User data is handled with strict privacy practices. No sensitive information is stored, and all inputs are processed securely.

6. Built for Continuous Improvement

As more data becomes available, the machine learning model will continue to improve. This ensures better accuracy and smarter recommendations over time.

📜 **License**

This project is open source and available under the MIT License.


**🛠️ Tech Stack**

Python

Flask

Scikit Learn

Pandas and NumPy

HTML, CSS, JavaScript

Pickle for model serialization

**Model Training**

Training Dataset: https://www.kaggle.com/datasets/noorsaeed/medicine-recommendation-system-dataset

**1. Data Loading and Preprocessing**

Key preprocessing steps include:

Reading the dataset and exploring its shape and unique prognosis values

Using LabelEncoder to convert the categorical prognosis column into numeric labels

Splitting the data into training and testing sets for model evaluation

This preprocessing ensures that the data is in a suitable format for machine learning algorithms.

2. Model Training

Five machine learning models were trained and evaluated:

Support Vector Classifier (SVC)

Random Forest Classifier

Gradient Boosting Classifier

K Neighbors Classifier

Multinomial Naive Bayes

Each model achieved 80 percent accuracy.

The SVC model was selected as the best performer for deployment.

3. Model Saving and Loading

To allow future use without retraining:

The trained SVC model is saved using pickle

The saved model is then loaded back and tested

This ensures the prediction pipeline works correctly even after saving and loading

4. Single Prediction

The loaded model is used to perform a single prediction on sample inputs.
This demonstrates how the system receives user symptoms, processes them, and returns a predicted disease label.

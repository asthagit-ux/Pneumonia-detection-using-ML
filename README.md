GitHub Repo stars GitHub forks contributors-shield LinkedIn

<br /> <p align="center"> <a href="https://github.com/rppradhan08/pneumonia-detection"> <img src="https://raw.githubusercontent.com/rppradhan08/pneumonia-detection/master/images/logo.PNG" alt="Logo" width="200px" height="100px"> </a> <p align="center"> <b>Pneumonia Detection Using CNN</b> <br /> <a href="https://github.com/rppradhan08/pneumonia-detection"><strong>Explore the docs »</strong></a> <br /><br /> <a href="https://github.com/rppradhan08/pneumonia-detection">View Demo</a> · <a href="https://github.com/rppradhan08/pneumonia-detection/issues">Report Bug</a> </p> </p>
Table of Contents
About The Project
Steps Involved
Tools Used
Getting Started
Installation
Data Analysis and Model Building
Application Development
Usage
Contact
About The Project
<p align="center"> <img src="https://raw.githubusercontent.com/rppradhan08/pneumonia-detection/master/images/person1661_virus_2872.jpeg" height="250px" width="300px"> </p>
This web application leverages a Convolutional Neural Network (CNN) built and trained using the Keras API to detect pneumonia from chest X-ray images. The model is integrated into a Flask-based web app for easy end-user interaction.

The Chest X-Ray dataset used is sourced from Kaggle, containing 5,863 X-ray images categorized as Pneumonia or Normal, structured into train, validation, and test sets.

Steps Involved
Data loading and preprocessing with OpenCV.
Data augmentation to improve generalization and reduce overfitting.
Sequential CNN model construction using Keras.
Model training, evaluation, and metrics computation.
Deployment as a Flask web application for real-time X-ray analysis.
Tools Used
Python
Keras
Flask
OpenCV
HTML
CSS
Getting Started
Installation
Create a virtual environment and install the required dependencies:

bash
pip install -r requirements.txt
Data Analysis and Model Building
Refer to Pneumonia_Detection_CNN.ipynb for detailed data analysis and model-building steps.

Model Evaluation
To assess model performance, we use the Confusion Matrix and Classification Report, focusing on the following metrics:

Accuracy: Overall correctness of the model.
Precision: How many of the predicted pneumonia cases are actually pneumonia.
Recall (Sensitivity): How many actual pneumonia cases the model correctly identified.
F1-Score: Harmonic mean of precision and recall.
<p align="center"> <b>Confusion Matrix</b><br> <img src="https://raw.githubusercontent.com/rppradhan08/pneumonia-detection/master/images/cunfusion_mat.png" height="200px"> </p>
The model achieves strong results across these metrics, making it reliable for pneumonia detection in clinical settings.

Application Development
The trained CNN model is integrated into a Flask web application for user-friendly pneumonia detection from uploaded chest X-ray images. See app.py for implementation details.

Snapshots:

Step 1: Upload an X-ray

<p align="center"> <img src="https://raw.githubusercontent.com/rppradhan08/pneumonia-detection/master/images/home.PNG" height="300px"> </p>
Step 2: View Results

<p align="center"> <img src="https://raw.githubusercontent.com/rppradhan08/pneumonia-detection/master/images/normal.PNG" height="200px"> </p>
Usage
To launch the application, run:

bash
python app.py
Access the app at: http://127.0.0.1:5000/


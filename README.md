# Phishing URL Detection and NLP Based Chatbot
This repository contains the project **"Phishing URL Detection and NLP-Based Chatbot"**, which integrates machine learning and natural language processing to detect phishing websites and provide a multilingual chatbot for user interaction.

## Table of Content
  * [Introduction](#introduction)
  * [Installation](#installation)
  * [Features](#features)
  * [Directory Tree](#directory-tree)
  * [Technologies Used](#technologies-used)
  * [Result](#result)
  * [Conclusion](#conclusion)


## Overview
The project aims to:
1. **Detect Phishing URLs**: Use machine learning to determine whether a given URL is genuine or fraudulent.
2. **Multilingual Chatbot**: Provide a chatbot capable of responding to user queries in English, Hindi, and Marathi.

The application also includes a user interface where users can paste a link to verify its authenticity and interact with the chatbot for assistance.


## Installation
The Code is written in Python 3.6.10. If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:
```bash
pip install -r requirements.txt
```

## Features
- **Phishing Detection**:
  - Employs XG-Boost machine learning algorithm with an accuracy of 97%.
  - Dataset of 10,000 URLs for training and testing.

- **Multilingual Chatbot**:
  - Developed using Dialogflow.
  - Supports English, Hindi, and Marathi.

- **User Interface**:
  - Allows users to paste URLs to verify them.
  - Interactive chatbot interface.

## Directory Tree 
```
├── pickle
│   ├── model.pkl
│   ├── rf_model.pkl
├── static
│   ├── styles.css
├── templates
│   ├── index.html
├── Phishing URL Detection.ipynb
├── app.py
├── app1.py
├── feature.py
├── phishing.csv
├── Procfile
├── README.md
├── requirements.txt


```

## Technologies Used
- **Backend**:
  - Python
  - Flask
  - XG-Boost (Machine Learning)

- **Frontend**:
  - HTML, CSS, JavaScript, Bootstrap

- **Chatbot**:
  - Dialogflow

- **Database**:
  - SQLite for storing user interactions.


## Result

Accuracy of various model used for URL detection
<br>

<br>

||ML Model|	Accuracy|  	f1_score|	Recall|	Precision|
|---|---|---|---|---|---|
0|	Gradient Boosting Classifier|	0.974|	0.977|	0.994|	0.986|
1|	CatBoost Classifier|	        0.972|	0.975|	0.994|	0.989|
2|	XGBoost Classifier| 	        0.969|	0.973|	0.993|	0.984|
3|	Multi-layer Perceptron|	        0.969|	0.973|	0.995|	0.981|
4|	Random Forest|	                0.967|	0.971|	0.993|	0.990|
5|	Support Vector Machine|	        0.964|	0.968|	0.980|	0.965|
6|	Decision Tree|      	        0.960|	0.964|	0.991|	0.993|
7|	K-Nearest Neighbors|        	0.956|	0.961|	0.991|	0.989|
8|	Logistic Regression|        	0.934|	0.941|	0.943|	0.927|
9|	Naive Bayes Classifier|     	0.605|	0.454|	0.292|	0.997|


## Conclusion
- The project successfully integrates machine learning and NLP to address two key problems: phishing URL detection and multilingual chatbot interaction.
- It achieves high accuracy in phishing detection (97%) using an XG-Boost algorithm.
- The chatbot provides a seamless user experience in three languages, making it accessible to a broader audience.
- The user-friendly interface simplifies the process of checking URLs and interacting with the chatbot.
- This application can be further improved with additional features, making it a robust tool for cybersecurity and user assistance.

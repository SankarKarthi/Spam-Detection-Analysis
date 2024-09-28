# Spam Detection System

## Overview
This project is a simple **Spam Detection System** built using Python, `scikit-learn`, and `Streamlit`. It classifies text messages (such as emails or SMS) as either "spam" or "ham" (non-spam) using a **Naive Bayes classifier**. The system leverages **CountVectorizer** to convert the text data into a numerical format that can be processed by machine learning algorithms.

## How it Works
1. The system loads a dataset of SMS messages labeled as "spam" or "ham" from a CSV file (`spam.csv`).
2. The **CountVectorizer** is used to transform the text data into a numerical form, where each word in the message is counted.
3. A **Multinomial Naive Bayes classifier** is trained on the vectorized text data.
4. Users can input a message into the Streamlit app, and the trained model predicts whether the message is spam or not.

## Features
- **Text Preprocessing**: Uses `CountVectorizer` to convert messages into a bag-of-words representation.
- **Naive Bayes Classifier**: The system applies a **Multinomial Naive Bayes** classifier to categorize messages.
- **Streamlit UI**: A simple and interactive web interface built with Streamlit to make predictions.

## Dataset
The dataset used is `spam.csv`, which contains two columns:
- `Category`: Label indicating if the message is "spam" or "ham".
- `Message`: The text content of the message.

## Installation and Setup

1. Clone the repository to your local machine:
    ```bash
    git clone https://github.com/yourusername/spam-detection-system.git
    ```

2. Navigate to the project directory:
    ```bash
    cd spam-detection-system
    ```

3. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Run the Streamlit app:
    ```bash
    streamlit run main.py
    ```

## Requirements

To run this project, you will need the following libraries:
- `pandas`
- `numpy`
- `scikit-learn`
- `streamlit`

You can install all required packages by running:
```bash
pip install -r requirements.txt

# 📧 Email Spam Filtering System

This project is a powerful, efficient, and easy-to-use **Email Filtering System** that identifies spam emails using advanced machine learning techniques. It delivers fast and accurate results for users through a user-friendly web interface.

---

## 🔍 Project Overview

The goal of this project was to create a **spam detection system** capable of classifying emails as either spam or non-spam (ham) using a supervised learning model. The backend is powered by Flask, with a clean, responsive frontend for easy interaction.

---

## ⚙️ Model Training

I utilized a supervised machine learning approach to train the model. Below are the steps and techniques I followed:

- **Data Preprocessing**:  
  Cleaned the email texts by removing stop words, punctuation, and applied tokenization.
  
- **TF-IDF Vectorization**:  
  Text was converted into numerical vectors using **Term Frequency-Inverse Document Frequency (TF-IDF)** to make it processable by the machine learning model.

- **Machine Learning Model**:  
  After testing multiple models, I selected **Naive Bayes** for its simplicity and effectiveness in text classification. It works particularly well for spam detection by leveraging word frequency and probability.

- **Evaluation Metrics**:  
  Measured the performance using **accuracy, precision, recall**, and **F1 score**, achieving **95%+ accuracy** in detecting spam emails.

- **Cross-validation**:  
  Applied cross-validation to ensure the model generalizes well and avoids overfitting.

---

## 🖥️ Backend (Powered by Flask)

The backend is built using the Flask framework, providing a robust system for handling email filtering:

- **Model Integration**:  
  The trained model is serialized using **joblib** for easy integration into the Flask backend, allowing it to predict whether an email is spam or ham.

- **User Authentication**:  
  Added **login and signup** functionality using Flask-Login, so users can create accounts and access their personal spam-filtering dashboard.

- **Database**:  
  Integrated **SQLite** for storing user data, including credentials and a history of email filtering.

- **API for Predictions**:  
  The backend includes a prediction **API** that processes the incoming email text and returns whether it's spam or ham.

---

## 🎨 Frontend (Responsive and User-Friendly)

The frontend was designed with usability in mind, providing a smooth and modern experience for users:

- **HTML/CSS/JavaScript**:  
  Developed using **HTML5, CSS3, and JavaScript** to create a responsive and intuitive interface.

- **Login & Signup Pages**:  
  Created sleek, modern forms for user authentication.

- **Dashboard**:  
  Users can input emails and receive real-time feedback on whether an email is spam or ham through their **personal dashboard**.

- **Pop-ups and Alerts**:  
  Integrated JavaScript-based **alerts** and feedback messages to enhance the user experience.

---

## 💻 Tech Stack

- **Machine Learning**: Python (Naive Bayes, Scikit-learn)
- **Web Framework**: Flask
- **Frontend**: HTML5, CSS3, JavaScript
- **Database**: SQLite
- **Model Deployment**: joblib

---

## 🚀 Installation and Setup

Follow these steps to set up the project on your local machine:

### Prerequisites

- Python 3.x
- Flask
- Scikit-learn
- joblib

### Steps

1. **Clone the repository**:
    ```bash
    git clone https://github.com/yourusername/email-spam-filter.git
    cd email-spam-filter
    ```

2. **Create a virtual environment** (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # For Windows: venv\Scripts\activate
    ```

3. **Install the dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Flask application**:
    ```bash
    python app.py
    ```

5. **Access the web app**:  
   Open your browser and go to:  

# Chrome_extension-_youtube-_Comment-_Sentiment_UsingML

# 🧠 YouTube Comment Sentiment Analyzer - Chrome Extension (with Flask API)

An end-to-end project that combines **Machine Learning**, **Chrome Extension development**, and **Cloud Deployment** to analyze YouTube comments in real-time. This tool allows users to instantly see the sentiment (positive/negative) of comments on any YouTube video using a browser extension backed by a trained LightGBM model served via a Flask API.

---

## 📖 Project Description

In today’s digital age, user-generated content like YouTube comments offers a wealth of insight into viewer sentiment. Manually reading through thousands of comments is time-consuming and inefficient.

This project solves that problem by:
- Using **Machine Learning** to predict sentiment from YouTube comments.
- Building a **Chrome Extension** that overlays sentiment scores directly in the browser.
- Hosting a **Flask API** to serve the ML model.
- Leveraging **MLflow** to track and monitor experiments.
- Deploying the entire application using **AWS services** with a fully automated **CI/CD pipeline via GitHub Actions**.

This solution is ideal for:
- Content creators monitoring engagement
- Researchers analyzing public opinion
- ML enthusiasts learning real-world deployment

---

## 📌 Project Workflow

1. **Dataset Collection & Preprocessing**
   - Cleaned YouTube comment text
   - Removed stopwords, symbols, and converted to lowercase

2. **Exploratory Data Analysis (EDA)**
   - Distribution of sentiments
   - Word frequency, bigrams, etc.

3. **Model Training & Experimentation (Jupyter Notebook)**
   - Tried multiple models:
     - Logistic Regression
     - Decision Tree
     - Random Forest
     - LightGBM ✅ (Best performance)
   - Evaluation metrics:
     - Accuracy, F1-score, ROC AUC, R²

4. **Hyperparameter Tuning**
   - Used GridSearchCV / RandomizedSearchCV
   - Best model logged in **MLflow**

5. **Model Serving with Flask API**
   - RESTful endpoint to predict sentiment on comments
   - Accepts JSON input and returns prediction

6. **Chrome Extension Frontend**
   - Fetches YouTube video comments
   - Sends to Flask API
   - Displays predicted sentiment inside the popup

7. **CI/CD & Deployment (AWS)**
   - Model + API containerized using Docker
   - Pushed to **ECR**
   - Deployed to **EC2**
   - Managed using **GitHub Actions**

---

## 🛠️ Tech Stack

- **ML**: LightGBM, Scikit-learn, Pandas, NumPy
- **Model Serving**: Flask
- **Frontend**: Chrome Extension (HTML, JS, CSS)
- **Experiment Tracking**: MLflow (hosted on AWS)
- **CI/CD**: GitHub Actions
- **Cloud Infra**: AWS (EC2, ECR, S3)

---

## 💻 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/youtube-sentiment-extension.git
cd youtube-sentiment-extension

<<<<<<< HEAD
python -m venv youtube_env

youtube_env\Scripts\activate

pip install -r requirements.txt

## DVC

dvc init

dvc repro

dvc dag


107544175286.dkr.ecr.us-east-1.amazonaws.com/mlproject
=======
chrome://extensions/
>>>>>>> 3add729cde542563e7606fe2d6706fe4b9820f0a

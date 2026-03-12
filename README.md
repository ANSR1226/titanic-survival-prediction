# 🚢 Titanic Survival Prediction (Streamlit App)

Predict whether a passenger would have survived the Titanic using a machine learning model wrapped in an interactive Streamlit app.

***

## 🌐 Live Demo

> Deployed on Streamlit: `https://your-app-url.streamlit.app`  
_Update this with your real link._

***

## 📌 Project Overview

This project tackles the classic Titanic dataset and builds an end‑to‑end machine learning pipeline to predict passenger survival.  
The final model is deployed as a Streamlit web app where users can adjust inputs (age, ticket class, fare, etc.) and instantly see the predicted outcome and probability. [github](https://github.com/ZG3Z/Streamlit-Titanic-Prediction)

***

## ✨ Features

- Interactive **web interface** built with Streamlit for real‑time predictions. [github](https://github.com/cedanl/streamlit-app-template)
- End‑to‑end **ML pipeline**: preprocessing, feature engineering, and a trained classifier (e.g., RandomForestClassifier).  
- Input controls for:
  - Passenger class (Pclass)  
  - Age, sex, number of siblings/spouses (SibSp), number of parents/children (Parch)  
  - Fare  
  - Embarked port  
- Prediction output: **Survived / Not Survived** plus model probability.  

***

## 🧠 Model & Data

- Dataset: Titanic passenger data (Kaggle’s “Titanic: Machine Learning from Disaster”).  
- Target: `Survived` (1 = survived, 0 = did not survive).  
- Example preprocessing steps:
  - Handling missing values  
  - Encoding categorical variables (sex, embarked, class)  
  - Selecting useful features  
- Model: scikit‑learn classifier (e.g., RandomForestClassifier) trained on the processed features. [github](https://github.com/Melo04/titanic-survival-prediction)

You can inspect the full workflow in the notebook: `titanic_survive.ipynb` (or your actual notebook name).

***

## 🏃 How to Run Locally

1. **Clone the repository**

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. **Create a virtual environment (optional but recommended)**

```bash
python -m venv .venv
# Windows
.\.venv\Scripts\activate
# macOS/Linux
source .venv/bin/activate
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

4. **Run the Streamlit app**

```bash
streamlit run app.py
```

5. Open the URL that appears in your terminal.

***

## 📂 Repository Structure

```text
.
├── app.py                 # Streamlit app
├── titanic_model.pkl      # Trained ML model (joblib)
├── titanic.csv            # Dataset (or data/ folder)
├── titanic_survive.ipynb  # Training & exploration notebook
├── requirements.txt       # Project dependencies
└── LICENSE                # MIT license
```

***

## 🚀 Deployment

This app is deployed on **Streamlit Community Cloud**:

- The app pulls code and `titanic_model.pkl` directly from this GitHub repository.
- `requirements.txt` pins versions for Streamlit, scikit‑learn, numpy, pandas, and joblib to ensure the model loads correctly on the server.
You can fork this repo and deploy your own version by connecting it to Streamlit Cloud.

***

## 🧪 Future Improvements

- Try different models (Gradient Boosting, XGBoost, etc.) and compare performance.  
- Add model evaluation plots (ROC curve, confusion matrix).  
- Log predictions for basic analytics.  
- Improve the UI with better layout, explanations, and example inputs.

***

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

- Fork the repo  
- Create a new branch: `git checkout -b feature/my-feature`  
- Commit your changes and open a pull request

***

## 📜 License

This project is licensed under the **MIT License**.  
See `LICENSE` for details.
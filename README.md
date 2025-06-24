# Diabetes Prediction App

This project is a **Diabetes Prediction Web Application** built using a Machine Learning model trained on a healthcare dataset. Users can input key health parameters (e.g. Glucose, BMI, Age, Pregnancies), and the app predicts their likelihood of having diabetes.

The solution consists of:
- A **Jupyter Notebook** for data exploration, model training & evaluation.
- 
- A **Streamlit** app for a user-friendly interface to make predictions.

- ## Key Features
- Loads a pre-trained Diabetes model and scaler.
- Scales user inputs and provides real-time diabetes risk predictions.
- Displays the predicted outcome with confidence level.
- Interactive interface powered by Streamlit.

## Dataset
This project is trained on the **Pima Indians Diabetes Dataset** containing features such as:
- Glucose
- BMI
- Age
- Pregnancies

You can obtain the dataset from [UCI Machine Learning Repository](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database?select=diabetes.csv).


## Model Development
1. **Preprocessing**: Features were scaled using `StandardScaler`.
2. **Model Training**: A `LogisticRegression` model was trained and saved with `joblib`.
3. **Evaluation**:
   - Accuracy: `~80%`
   - Confusion Matrix and metrics were calculated.
  
   - ## Streamlit Application
Run the `stremlit_app_2.py` file to launch a local web app:
```bash
streamlit run stremlit_app_2.py

You will see:

Input fields for Glucose, BMI, Age, Pregnancies.

A "Prediction" button that returns:

Diabetic or Not Diabetic

Prediction confidence (probability score)

# Wine Classification Using MLflow

## 1. Project Overview

This project implements a Wine Classification Machine Learning workflow using MLflow for experiment tracking and model registration.

It trains and compares three machine learning algorithms:
- Logistic Regression
- Decision Tree
- Random Forest

The models are evaluated using Accuracy, Precision, Recall, and F1-score. The best-performing model is registered in MLflow and used to make predictions.

## 2. Technologies Used

- Python
- Scikit-learn
- MLflow
- NumPy
- Pandas
- Git and GitHub

## 3. Project Structure

```text
MLOps_Flow-member-6/
│
├── generate_wine.py
├── train.py
├── register_model.py
├── predict.py
├── requirements.txt
└── .gitignore
```

## 4. Project Workflow

1. Generate the Wine dataset.
2. Train three machine learning models.
3. Track model parameters and evaluation metrics using MLflow.
4. Compare model performance.
5. Register the best-performing model.
6. Load the registered model and perform predictions.

## 5. Installation

Clone the repository:

```bash
git clone https://github.com/khushi13-tech/MLOps_Flow-member-6.git
```

Open the project folder:

```bash
cd MLOps_Flow-member-6
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

## 6. How to Run the Project

**Step 1: Generate the dataset**

```bash
python generate_wine.py
```

**Step 2: Start the MLflow server**

```bash
python -m mlflow server --host 127.0.0.1 --port 5000 --backend-store-uri sqlite:///mlflow.db
```

Keep this terminal running.

**Step 3: Train the models**

Open another terminal and run:

```bash
python train.py
```

**Step 4: Register the best model**

```bash
python register_model.py
```

**Step 5: Make predictions**

```bash
python predict.py
```

## 7. MLflow Tracking

MLflow is used to track:
- Model parameters
- Accuracy
- Precision
- Recall
- F1-score
- Trained model artifacts

Open the MLflow dashboard in your browser:

http://127.0.0.1:5000

## 8. Evaluation Metrics

The models are evaluated using:

- **Accuracy:** Measures overall correct predictions.
- **Precision:** Measures how many positive predictions are correct.
- **Recall:** Measures how many actual positive cases are identified.
- **F1-score:** Represents the balance between precision and recall.

## 9. Conclusion

This project demonstrates an end-to-end machine learning workflow using MLflow. It helps compare multiple classification algorithms, track their performance, register the best model, and perform predictions.

---

**Project:** Wine Classification Using MLflow  
**Repository:** MLOps_Flow-member-6

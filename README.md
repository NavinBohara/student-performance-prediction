# EduPredict AI – Unlocking Student Potential with AI

![Streamlit](https://img.shields.io/badge/Streamlit-App-orange) ![TensorFlow](https://img.shields.io/badge/TensorFlow-Deep_Learning-red) ![Python](https://img.shields.io/badge/Python-3.8+-blue)

---

## Overview

**EduPredict AI** is an interactive web application built with Streamlit that predicts student performance in Math, Reading, and Writing based on demographic and educational background data. The app employs a Multi-Task Learning (MTL) deep learning model using TensorFlow to simultaneously predict scores across three subjects.

The system also features a simple login authentication, data preprocessing, visualization of predictions, and allows users to predict scores for new student profiles.

---

## Features

- **Login System:** Basic username-password authentication for access control.
- **Data Upload:** Upload CSV dataset (`StudentsPerformance.csv`) for model training and evaluation.
- **Data Preprocessing:** Encodes categorical variables, splits data, and scales features.
- **Multi-Task Learning Model:** Simultaneous prediction of Math, Reading, and Writing scores using a shared neural network architecture.
- **Training & Evaluation:** Train the model and visualize training progress.
- **Prediction Visualization:** Correlation heatmap and scatter plots for actual vs. predicted scores.
- **Custom Prediction:** User-friendly form to input new student details and get predicted scores.
- **Classification Report:** Displays classification metrics in a table format for model assessment.

---

## Installation

### Prerequisites

- Python 3.8 or higher
- Recommended: Virtual environment setup (venv or conda)

### Required Libraries

```bash
pip install streamlit pandas numpy tensorflow scikit-learn seaborn matplotlib




## Usage

1. **Run the Streamlit App:**

```bash
streamlit run edupredict_app.py
```

2. **Login Credentials:**

* Username: `admin`
* Password: `password`

3. **Upload Dataset:**

* Upload your `StudentsPerformance.csv` file via the sidebar.

4. **View Dataset & Classification Report:**

* Preview the data and classification report on the main page.

5. **Train the Model:**

* The model trains automatically after uploading the dataset.

6. **View Predictions & Visualizations:**

* Correlation heatmap and scatter plots display model performance.

7. **Predict for New Students:**

* Use the form to enter new student info and get predicted Math, Reading, and Writing scores.

---

## Dataset

The model expects a dataset with the following features:

* `gender`
* `race/ethnicity`
* `parental level of education`
* `lunch`
* `test preparation course`
* `math score`
* `reading score`
* `writing score`

Ensure the CSV columns match these names (case-insensitive). The app renames some columns internally for consistency.

---

## Model Architecture

* Input layer accepts encoded categorical features.
* Two shared dense layers with ReLU activation.
* Three output layers for each subject score (`math_output`, `reading_output`, `writing_output`).
* Loss function: Mean Squared Error for all outputs.
* Optimizer: Adam with learning rate 0.01.

---

## Folder Structure Suggestion

```
EduPredict-AI/
│
├── StudentsPerformance.csv       # Sample dataset
├── edupredict_app.py             # Streamlit app script (your main code)
├── requirements.txt              # Python dependencies
└── README.md                    # Project documentation
```

---

## Future Improvements

* Enhance login system with hashed passwords and user management.
* Add real-time model training progress visualization.
* Extend dataset with more features for better accuracy.
* Deploy as a web service for public access.
* Integrate advanced metrics and model explainability.

---

## Author

**Your Name**
Email: navinbohara5@gmail.com
GitHub: https://github.com/NavinBohara

---

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

* Dataset from [Kaggle Student Performance Dataset](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams)
* Thanks to TensorFlow, Streamlit, and Scikit-learn communities for their amazing tools!

---

**Enjoy predicting and unlocking student potential with EduPredict AI! 🚀**

```

---

Just replace **Your Name**, email, and GitHub link with your details, and you’re good to go! Need help with anything else?
```

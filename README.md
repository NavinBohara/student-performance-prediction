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

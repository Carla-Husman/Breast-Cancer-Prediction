# Breast Cancer Prediction – C# / AI Project

This repository contains an Artificial Intelligence project developed in the 4th year of university.  
The goal of the project is to build and evaluate a model that **predicts whether a breast tumor is malignant or benign** based on tabular medical data.

---

## Project Overview

The application explores how different **parameter configurations** and **model choices** impact prediction performance on a breast cancer dataset.

Main ideas:

- Load and process a real-world **breast cancer dataset**.
- Train and evaluate one or more **machine learning models**.
- Experiment with **different parameter configurations** and compare results.
- Visualize and interpret metrics to understand which configuration works best.

---

## Tech Stack

- **Language:** C# (≈ 86% of the code), Python (≈ 14% of the code)
- **Platform:** .NET / Visual Studio
- **Paradigms:** Object-Oriented Programming, basic AI / ML workflow
- **Extras:** 
  - Data loading & preprocessing
  - Metrics computation and comparison
  - Separate project for parameter selection / experimentation

---

## Repository Structure

At a high level, the repository contains:

- `BreastCancer/`  
  Main C# project that loads the dataset, runs the AI model(s) and computes metrics.

- `Alegere parametri/`  
  Parameter selection / experimentation project. Used to test different hyperparameter configurations and compare their impact.

- `Documentație.pdf`  
  Project documentation (in Romanian) describing the problem, method and results in more detail.

---

## Features

- Load and validate input data from a breast cancer dataset.
- Train a machine learning model to classify tumors (benign vs malignant).
- Configure and compare **multiple parameter sets** (e.g. thresholds, learning-related options, etc.).
- Display evaluation metrics (accuracy and/or other metrics, depending on the implementation).
- Clear separation between:
  - the **core breast cancer prediction logic** and  
  - the **parameter selection / experimentation** part.

---

## Getting Started

### Prerequisites

- **Visual Studio** (or another IDE with C#/.NET support)
- **.NET SDK** installed
- (Optional) **Python 3** and required ML libraries, if you want to run the Python side of the project

### How to Run

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Carla-Husman/Proiect-IA.git
   cd Proiect-IA
   ```

2. **Open the C# solution/project** inside the `BreastCancer` folder in Visual Studio.

3. **Restore and build** the project from Visual Studio.

4. **Run** the application (F5 or “Start Debugging”).

5. (Optional) Open the `Alegere parametri` project to experiment with different configurations / hyperparameters and compare the results.

> If your environment or dataset path is different, you may need to update the file paths inside the code (for example where the dataset is loaded).

---

## How It Works (High-Level)

1. **Data loading**  
   The application loads the breast cancer dataset from a file and converts it into an internal representation suitable for training and evaluation.

2. **Preprocessing**  
   Basic cleaning / transformation of data (e.g. handling missing values, converting text to numeric, normalizing features – depending on implementation).

3. **Modeling**  
   A machine learning model is configured and trained to classify each record as benign or malignant.

4. **Evaluation**  
   The model is evaluated on a test set and metrics are computed (for example, classification accuracy).  
   In the parameter selection project, **multiple configurations** are tested and compared.

# ☁️ AWS SageMaker - Mobile Price Classification Project

This project is focused on building a machine learning classification model that predicts whether a mobile phone falls into a low or high price category based on various features. The primary goal is to prepare the model for deployment on **Amazon SageMaker**, a powerful cloud-based ML platform that automates training, tuning, and deployment.

The dataset used in this project contains mobile phone specifications such as battery power, RAM, screen width/height, number of cores, 4G/3G availability, and more. Each phone is labeled as either priced low or high, making this a **binary classification problem**.

The project follows the typical end-to-end ML workflow:

1. **Exploratory Data Analysis (EDA):** Performed in `research.ipynb` to understand distributions, correlations, and missing values.
2. **Preprocessing:** The dataset is cleaned and preprocessed. It is then split into training (`train-V-1.csv`) and testing (`test-V-1.csv`) sets.
3. **Model Development:** The classification model is implemented using a script (`script.py`) which is compatible with AWS SageMaker’s training architecture.
4. **Deployment Readiness:** The script is designed to be uploaded to SageMaker, where you can use the SKLearn estimator to perform training, evaluation, and real-time inference setup.

The project structure is kept minimal and clean for fast integration into SageMaker pipelines. This is an ideal starter template for anyone wanting to deploy simple classification models using AWS cloud tools.

No web frontend or API endpoint has been integrated in this version of the project, as the focus remains on preparing the training pipeline for SageMaker.

This setup serves as a practical demonstration of using SageMaker for cloud-based ML lifecycle management, including dataset handling, model training, and deployment at scale.

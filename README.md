# IBM Attrition Predictor
![bg](https://github.com/user-attachments/assets/f3046f5d-8a6e-483a-ad35-d1d0583ecfbe)

## Dataset 
https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset

## Features

- Data Preprocessing and EDA
- Model Training and Evaluation (Logistic Regression, MLP, XG-Boost)
- Training Pipeline
- Inference Pipeline
- Data Ingestion and Transformation
- Model Trainer
- Hyperparameter Tuning
- Automatic Data Augmentation
- Docker Image Creation Script
- CI/CD Workflow (GitHub Actions to Amazon ECR to Amazon EC2)
- Reverse Proxy Setup for HTTPS Requests
- SSL & TLS Certificates

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/IBM_Attrition_Predictor.git
    ```
2. Navigate to the project directory:
    ```sh
    cd IBM_Attrition_Predictor
    ```
3. Create a virtual environment:
    ```sh
    python -m venv venv
    ```
4. Activate the virtual environment:
    - On Windows:
        ```sh
        venv\Scripts\activate
        ```
    - On macOS/Linux:
        ```sh
        source venv/bin/activate
        ```
5. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

## Usage

### Data Preprocessing and EDA

1. Open the Jupyter notebook for EDA:
    ```sh
    jupyter notebook src/notebooks/EDA.ipynb
    ```
2. Run the cells to preprocess the data and perform exploratory data analysis.

### Model Training

1. Open the Jupyter notebook for model training:
    ```sh
    jupyter notebook src/notebooks/models.ipynb
    ```
2. Run the cells to train the models and evaluate their performance.

### Model Deployment

1. Navigate to the [`backend`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fdebop%2FDesktop%2FData%20Science%2FIBM%20Attrition%20Predictor%2Fbackend%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%2C%22bbc7cc02-5494-4456-869e-a09f88b89bb5%22%5D "c:\Users\debop\Desktop\Data Science\IBM Attrition Predictor\backend") directory:
    ```sh
    cd backend
    ```
2. Run the backend server:
    ```sh
    fastapi dev main.py
    ```

## CI/CD Workflow

This project includes a CI/CD workflow using GitHub Actions to build and deploy Docker images to Amazon ECR and then to an Amazon EC2 instance. The workflow also sets up a reverse proxy on the server to handle HTTPS requests and manage SSL & TLS certificates.

## Configuration

The configuration settings are stored in the [`config/config.yaml`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fdebop%2FDesktop%2FData%20Science%2FIBM%20Attrition%20Predictor%2Fconfig%2Fconfig.yaml%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%2C%22bbc7cc02-5494-4456-869e-a09f88b89bb5%22%5D "c:\Users\debop\Desktop\Data Science\IBM Attrition Predictor\config\config.yaml") file. You can modify this file to change the settings for the project.

## Logging

Logs are stored in the [`logs`](command:_github.copilot.openRelativePath?%5B%7B%22scheme%22%3A%22file%22%2C%22authority%22%3A%22%22%2C%22path%22%3A%22%2Fc%3A%2FUsers%2Fdebop%2FDesktop%2FData%20Science%2FIBM%20Attrition%20Predictor%2Flogs%22%2C%22query%22%3A%22%22%2C%22fragment%22%3A%22%22%7D%2C%22bbc7cc02-5494-4456-869e-a09f88b89bb5%22%5D "c:\Users\debop\Desktop\Data Science\IBM Attrition Predictor\logs") directory. Each log file is named with the timestamp of when it was created.

## License

This project is licensed under the Apache 2.0.

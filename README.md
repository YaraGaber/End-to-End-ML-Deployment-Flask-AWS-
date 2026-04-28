 End-to-End ML Deployment: Student Performance Prediction

This project demonstrates a complete **Machine Learning pipeline**, from data ingestion and transformation to model deployment on **AWS Elastic Beanstalk**. It predicts student performance based on various demographic and academic factors.

 Tech Stack
* **Language:** Python 3.x
* **Machine Learning:** CatBoost, Scikit-learn, Pandas, Numpy
* **Web Framework:** Flask
* **Cloud Deployment:** AWS Elastic Beanstalk
* **Server/Gateway:** Gunicorn & WSGI
* **Logging & Monitoring:** Custom logging and exception handling modules

 Project Structure
* `src/`: Modular code for Data Ingestion, Transformation, and Model Training.
* `application.py`: The Flask entry point for the web application.
* `artifacts/`: Stores pre-trained models (`model.pkl`) and preprocessing objects (`preprocessor.pkl`).
* `.ebextensions/`: Configuration files for AWS Elastic Beanstalk environment.
* `notebook/`: Jupyter notebooks for Exploratory Data Analysis (EDA) and initial prototyping.

 Deployment on AWS
The application is containerized and configured for **AWS Elastic Beanstalk**. 
- It uses a **Python 3.9+** environment.
- **WSGI** is configured via `.ebextensions` to handle production-grade traffic.
- The pipeline is designed for scalability and easy integration with CI/CD tools.

 How to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/YaraGaber/End-to-End-ML-Deployment-Flask-AWS-.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the application:
   ```bash
   python application.py
   ```

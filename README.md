# 🎓 Student Performance Prediction - Machine Learning Project

## 📝 Objective

The goal of this project is to develop a **predictive model** that estimates student performance based on demographic and academic factors, such as gender, parental education, and test scores. By following **industry-standard practices** in machine learning, this project serves as a hands-on demonstration of how to build and deploy a modular, production-ready ML pipeline. The key focus is on structuring the codebase, ensuring scalable and reusable components, and deploying the final model in a real-world environment using **AWS Elastic Beanstalk**.

## 🚀 Project Highlights

- **Industry Standards**: Demonstrates best practices for building a machine learning project, including **logging**, **error handling**, and **modular coding**.
- **Comprehensive Workflow**: Follows a complete ML pipeline, from **data ingestion** and **preprocessing** to **model training**, **evaluation**, and **deployment**.
- **Hands-on Deployment**: Deploys the model using **AWS Elastic Beanstalk** to simulate real-world production scenarios.
- **Scalable & Modular**: Designed to allow easy adjustments and future improvements with structured code components.

## 🗂 Dataset

The dataset used for this project tracks student performance and includes the following features:

- **gender**: Gender of the student
- **race_ethnicity**: Ethnicity group of the student
- **parental_level_of_education**: The highest level of education attained by the student's parent(s)
- **lunch**: Type of lunch the student receives (standard or free/reduced)
- **test_preparation_course**: Whether or not the student completed a test preparation course
- **math_score**: The student's score in mathematics
- **reading_score**: The student's score in reading
- **writing_score**: The student's score in writing

### Sample Data:

```csv
"gender","race_ethnicity","parental_level_of_education","lunch","test_preparation_course","math_score","reading_score","writing_score"
"female","group B","bachelor's degree","standard","none","72","72","74"
"female","group C","some college","standard","completed","69","90","88"
"female","group B","master's degree","standard","none","90","95","93"
```

## 📁 Project Structure

```
├── artifacts/
│   ├── data.csv               # Original dataset
│   ├── model.pkl              # Trained machine learning model
│   ├── preprocessor.pkl       # Data preprocessing pipeline
│   ├── train.csv              # Training data
│   ├── test.csv               # Test data
│
├── notebook/
│   ├── 1. EDA STUDENT PERFORMANCE.ipynb     # Exploratory Data Analysis
│   ├── 2. MODEL TRAINING.ipynb              # Model training and evaluation
│
├── src/
│   ├── components/
│   │   ├── data_ingestion.py                # Data ingestion script
│   │   ├── data_transformation.py           # Data preprocessing and transformation
│   │   ├── model_trainer.py                 # Model training and evaluation
│   ├── pipeline/
│   │   ├── train_pipeline.py                # Script to train the model pipeline
│   │   ├── predict_pipeline.py              # Script for model inference on new data
│   ├── utils/
│   │   ├── logger.py                        # Custom logging functionality
│   │   ├── exception.py                     # Error handling and custom exceptions
│   │   ├── utils.py                         # Helper functions
│
├── venv/                                    # Virtual environment
├── .gitignore                               # Git ignore file
├── application.py                           # Main application entry point for inference
├── requirements.txt                         # Required libraries
├── README.md                                # Project readme (you're reading this!)
├── setup.py                                 # Setup for packaging the project
```

## 🔨 Workflow & Key Steps

### Logging & Error Handling:

- Implemented robust logging mechanisms using the `logger.py` utility to track each step of the process.
- Designed custom exception handling in `exception.py` to manage runtime errors gracefully.

### Exploratory Data Analysis (EDA):

- Conducted exploratory analysis to understand the distribution of data, relationships between features, and feature importance in predicting student performance.

### Data Ingestion:

- Built a data ingestion pipeline that reads the raw dataset and splits it into training and testing sets.

### Data Transformation:

- Implemented a data preprocessing pipeline to handle missing values, encode categorical variables, and standardize numerical features.

### Model Training:

- Trained a CatBoost regression model to predict student performance scores using the transformed data.
- Saved the trained model as `model.pkl` and the preprocessor as `preprocessor.pkl` for future inference.

### Prediction Pipeline:

- Built a prediction pipeline to load the trained model and preprocessor to make predictions on new data.

### Deployment:

- Deployed the trained model on AWS Elastic Beanstalk for scalability and real-world inference.

## 🔧 Setup & Installation

### 1. Clone the Repository:

```bash
git clone https://github.com/your-repository-url.git
cd your-repository-folder
```

### 2. Install Dependencies:

```bash
pip install -r requirements.txt
```

### 3. Run the Training Pipeline:

```bash
python src/pipeline/train_pipeline.py
```

### 4. Run the Prediction Pipeline:

```bash
python src/pipeline/predict_pipeline.py
```

## 🌐 Deployment

The model is deployed on AWS Elastic Beanstalk, simulating a real-world production environment for inference and scalability. The model can process new data through an API and provide performance predictions.

## 🛠 Technologies Used

- **Programming Language**: Python
- **Machine Learning**: Scikit-learn, CatBoost
- **Deployment**: AWS Elastic Beanstalk
- **Data Visualization**: Matplotlib, Seaborn
- **Development Tools**: Git, Jupyter Notebooks

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/your-repository-url/issues).

## 📄 License

This project is licensed under the MIT License.


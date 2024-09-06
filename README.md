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


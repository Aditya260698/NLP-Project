# Resume Screening App using NLP

## Overview

The Resume Screening App is a powerful tool designed to streamline the hiring process by automatically screening and categorizing resumes using Natural Language Processing (NLP) techniques. This application leverages machine learning algorithms to analyze resume texts and categorize them into predefined job categories, facilitating the recruitment process for organizations.

## Features

- **Automated Resume Screening**: The app automatically screens and categorizes resumes based on their content, reducing manual effort and saving time for recruiters.
- **NLP-powered Classification**: Utilizes NLP techniques such as TF-IDF vectorization and K Nearest Neighbors (KNN) classification to accurately categorize resumes into predefined job categories.
- **User-friendly Interface**: Offers an intuitive user interface for uploading resumes and viewing categorized results, making it easy for recruiters to use.
- **High Accuracy**: Achieves high accuracy in categorizing resumes, ensuring reliable results for effective decision-making in the hiring process.
- **Customizable**: The app allows customization of job categories and tuning of classification parameters to adapt to specific recruitment needs.

## Getting Started

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Aditya260698/NLP-Project
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

### Usage

1. Data Preparation:
   - Prepare a dataset of resumes in CSV format, with columns for resume text and corresponding job categories.

2. Data Preprocessing:
   - Clean the resume text using the provided `cleanResume()` function to remove noise such as URLs, special characters, and non-ASCII characters.

3. Feature Extraction:
   - Utilize the `TfidfVectorizer` from scikit-learn to convert the cleaned resume text into TF-IDF vectors, which represent the importance of each word in the resume.

4. Model Training:
   - Split the TF-IDF vectors and corresponding job categories into training and testing sets using the `train_test_split` function.
   - Train a K Nearest Neighbors (KNN) classifier on the training data to learn patterns and relationships between resume texts and job categories.

5. Model Evaluation:
   - Use the trained classifier to predict job categories for resumes in the testing set.
   - Calculate the accuracy of the predictions using the `accuracy_score` function from scikit-learn.

6. Application Deployment:
   - Run the Flask web application (`app.py`) to deploy the Resume Screening App.
   - Upload resumes via the web interface and view categorized results.


## Acknowledgments

- Inspiration from [Resume Screening Tool Tutorial](https://www.youtube.com/watch?v=hG8K5h2J-5g&t=2424s), which served as a reference for building this app.

## Support

For any questions or issues, please [open an issue](https://github.com/Aditya260698/resume-screening-app/issues) on GitHub.

---

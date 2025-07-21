# FakeJobClassifier

A machine learning project for detecting fraudulent job postings using natural language processing (NLP) and classification models. This project was developed for the LIN340 Computational Linguistics course.

## Overview
This project analyzes job posting data to classify listings as fraudulent or legitimate. It uses a combination of text preprocessing, feature extraction, and machine learning models, with a focus on handling class imbalance and maximizing recall to reduce missed fraud cases.

## Workflow

1. **Data Preprocessing**
   - Lowercasing, punctuation/special character removal
   - Tokenization, stop word removal, lemmatization
   - Handling missing values and cleaning categorical columns
   - Binary encoding for relevant columns
   - Combining text columns into a single feature

2. **Feature Extraction**
   - Bag-of-Words (BoW) unigram model
   - TF-IDF (unigrams and bigrams)

3. **Handling Class Imbalance**
   - SMOTE oversampling for the minority (fraudulent) class

4. **Modeling**
   - Multinomial Naive Bayes (primary model)
   - Logistic Regression (baseline)
   - Neural Network (4-layer, with class weights and early stopping)
   - 80/20 stratified train/test split
   - 5-fold cross-validation

5. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1 Score, Confusion Matrix
   - Emphasis on high recall to minimize missed fraud cases

## Dataset
- [Recruitment Scam Dataset on Kaggle](https://www.kaggle.com/datasets/amruthjithrajvr/recruitment-scam)
- Downloaded using `kagglehub`

## Usage

1. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
2. **Run the notebook:**
   Open `FakeJobClassifier_EDA_and_Modelling.ipynb` in Jupyter or VSCode and run all cells.

## Main Files
- `FakeJobClassifier_EDA_and_Modelling.ipynb`: Main notebook with all code, analysis, and results.
- `FakeJobClassifier_Final_Report.pdf`: Full project report, including Abstract, Introduction, Methods, Results, and Discussion.

## Authors
- Marvin Roopchan, Aamid Mohsin, Christian Kevin Sidharta

## License
This project is for academic use only. 
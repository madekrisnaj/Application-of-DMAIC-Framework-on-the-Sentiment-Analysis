# Application-of-DMAIC-Framework-on-the-Sentiment-Analysis

This repository contains scraping and sentiment analysis code with the aim of making business recommendations using the DMAIC framework.

## Sentiment Analysis
Sentiment analysis is one of the popular tasks in the field of Natural Language Processing (NLP) and belongs to the category of learning that requires targeted learning (Supervised Learning). Sentiment analysis is actually a plain text classification task with a specific goal, namely to find out the sentiment of public opinion on a subject/object (example: HP products at Tokopedia). 

## DMAIC
DMAIC (Define, Measure, Analyze, Improve, Control) is a broadly structured problem solving procedure that
used in quality and quality improvement processes. It is often associated
with six sigma activities, and almost all implementations of six sigma
using the DMAIC process.

Each step in the cyclical DMAIC Process is required to ensure the best possible results. The process steps:

* **Define** the Customer, their Critical to Quality (CTQ) issues, and the Core Business Process involved.

* **Measure** the performance of the Core Business Process involved.

* **Analyze** the data collected and process map to determine root causes of defects and opportunities for improvement.

* **Improve** the target process by designing creative solutions to fix and prevent problems.

* **Control** the improvements to keep the process on the new course.


## What we need to prepare?
1.   **Data**

     The data used is the *** application review data obtained from scraping data on the google play store.

2.   **Environtmet**
      *   Python Version : 3.7.6
      *   Library : Pandas, Numpy, Matplotlib, Seaborn, Scikitlearn, Google-Play-Scraper, Sastrawi, Re, String.

## Data Preparation
The data provided from google play store are not clean yet. We have to cleaned up and feature selection before going to the sentiment analysis.
1.   **Data Cleaning & Preprocessing**

     Data cleaning and preprocessing procedure including :
     *    Lowercase
     *    Remove Number
     *    Remove Punctuation
     *    Remove Whitespace
     *    Remove ASCII and Unicode
     *    Remove Newline
     *    Stop Words
     *    Stemming
     *    Vectorization

2.   **Feature Selection**

     From the variables we already have, we need to add one more variable. The variable is a value which is a label of positive or negative sentiment. So, now we have 5              variables to enter the data analysis.

3.   **Labeling**
     *    As initial labeling, scores 1-3 are classified as negative label and 4-5 are classified as positive label.
     * Only 2 classification classes are used because the need for DMAIC is only 2 classes in the form of defective and non-defective data..

We only use data in 2021 period. After going through the process of cleaning, stop words, stemming, remove missing values and filter data, the data used is 30,119 data.

## Exploratory Data Analysis
![1111111](https://user-images.githubusercontent.com/83490369/128549277-95ee010d-b9c8-4591-8531-0f1448a86f44.PNG)


## Model
*    The classification model used is the SVM model and handling imbalance data by resampling.
*    After resampling, we use 9,500 data for negative and positive label.
![image](https://user-images.githubusercontent.com/83490369/128548359-d9f7a74d-9245-4a94-b8db-d46897a7f454.png)




# NLP Political Speeches
Goal: Classify political speeches as Democratic or Republican

## Author
Jose Miguel Montoro - jose@josemiguelmontoro.com

## Description
This project investigates how to train ML/deep learning models so that they're able to classify political speeches into Democratic or Republican.
The training data are labeled, historical political speeches by Democratic or Republican politicians, scraped from around the web.
So far, several _word vector representation models_ have been implemented: ngrams (Bag of Words) using scikit-learn CountVectorizer, TD-IDF with scikit-learn, SpaCy word vectors, FastText word vectors.
Various ML classification models have been applied as well (Logistic Regression, Naive Bayes, Support Vector Machines, Random Forest) as well as neural networks (multi-layer perceptron, convolutional neural network).
The ML model with best results is SVM with TD-IDF. The MLP approach also performed very well with TD-IDF.

## Structure
All temporary files are in the `data` folder. Vector models are in the `vectors` folder. Some python modules are in the `helpers` folder, they include utilities to help process the data and build and evaluate the models. All the code to extract the data, EDA, preprocess text and build and evaluate models is in the `notebooks` folder.

These are the steps that were followed to complete the project. Each step corresponds to one notebook.
1. a) Web Scraping from https://millercenter.org/
1. b) Web Scraping from https://www.americanrhetoric.com/
2. Text Pre-Processing
3. Exploratory Data Analysis
4. Vectorization and Classification Models
5. Neural Networks
6. Deep Learning models
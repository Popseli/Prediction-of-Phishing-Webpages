# Prediction of Phishing Webpages
The aim of this project is to develop a binary classifier for distinguishing phishing webpages from legitimate ones using URL and webpage structure based features. Phishing webpages are webpages of websites owned by attackers for the purpose of collecting users' sensitive information such as email addresses, passwords, bank account details etc. and use it to impersonate victims in order to undertake various malicious activities including theft of money, execution of other cyberattacks and cyberespionage. Since phishing webpages highly resemble with legitimate webpages that prompt sensitive information, users find it difficult to distinguish the two, leading to most users even those with cybersecurity awareness to fall into the phishing attacks. The significance of this project, therefore, is to build an automated ML based mechanism that can exploit key differences in the structures of the two types of webpages to automatically detect the former, thus, protecting online users from the attacks. The ML model can be used to build an application that can be deployed as a built web browser feature or web browser plug in to offer protection at the time user is attempting to access any webpage that prompts for sensitive information. This project was part of my PhD research work.

## Objectives
To achieve the aim stated above, the following tasks were to be performed:
* Investigating and identifying potential webpage structure based features for distinguishing the two types of webpages.
* Extracting the features from realible data sources of phishing and legitimate webpages.
* Identify the most relevant feature set for the prediction task.
* Evaluating the relevant feature set using various ML classification algorithms to identify the best performing algorithm based on the performances reported by a wide range of metrics.
* Performing model explainability analysis to learn the influence of each feature on the model's output.

## Tasks Performed
* Retrieving sets of active phishing and legitimate webpages from online repositories.
* Creating a dataset by extracting feature values from the webpages.
* Understanding data descriptions and statistics.
* Performing data cleaning
* Performing data exploration analysis
* Feature correlation analysis
* Feature selection
* Model evalution
* ROC analysis
* Hyperparameter tuning
* Model explainability analysis

## Features
A total of 35 features based on URL and webpage structure, webpage contents and third party information related to a webpage were identified.

## Dataset
We retrieved 12,691 phishing and 13,494 legitimate webpages that prompt sensitive information from PhishTank and Tranco online repositories. From each active webpage, we extracted feature values to form a dataset of 26,115 records. The records were stored in a MySQL database.

## Key Software and Libraries Used
* Python
* Numpy
* Pandas
* MySQL
* Geoip2
* Google and Bing search engines
* Google Translator
* PhishTank
* Beautiful soup
* Matplotlib
* Seaborn
* Category encoders
* Recursive feature elimination with cross validation (RFECV)
* Algorithms: Logistic Regression, kNN, Decision Tree, Naive Bayes, SVM, Neural Networks (MLP), Random Forest, Gradient Boosting, LightGBM, XGBoost
* Repeated stratified cross validation
* Random search with cross validation (RandomizedSearchCV)
* SHAP

## Result Summary
XGBoost was observd to outperform other algorithms across most metrics by achieving an accuracy of 98.6 %, FPR of 1.12 % and FNR of 1.72 %. After tuning its hyperparameters, the algorithm's performance was optimized to achieve an accuracy of , FPR of and FNR of 

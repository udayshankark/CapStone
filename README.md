### Project Title
Fake News Detection using Machine Learning Techniques

**Author**
Uday Kemburu

#### Executive summary
This project implements and evaluates multiple machine learning models for fake news detection, achieving over 98% accuracy across different approaches. The best-performing model (Logistic Regression with lemmatization) achieved 99.32% accuracy on the test set, demonstrating the effectiveness of machine learning in distinguishing between real and fake news articles.

#### Rationale
This research is crucial in today's digital age where misinformation spreads rapidly and can have serious societal consequences. Developing effective automated tools for fake news detection can help:
1. Support fact-checkers and journalists in their work
2. Assist social media platforms in content moderation
3. Real-time fact-checking during political events

#### Research Question
Can machine learning models effectively distinguish between fake and real news articles based on textual features alone?

#### Data Sources
The analysis uses the Fake and Real News Dataset from Kaggle, containing:

23,502 fake news articles
21,417 real news articles
Features include: title, text, subject, date
Average text length: 2,537 characters
https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset

#### Methodology
What methods are you using to answer the question?
Text Preprocessing:

Lemmatization using NLTK
TF-IDF vectorization
Stop words removal


Models Implemented:

Logistic Regression (baseline and with lemmatization)
Support Vector Machine (SVM)
Decision Tree
Naive Bayes


Model Optimization:

Grid Search CV for hyperparameter tuning
5-fold cross-validation
Feature engineering through text preprocessing

#### Results
Model Performance:

Logistic Regression (baseline): 98.65% test accuracy
SVM: 99.21% test accuracy
Logistic Regression (with lemmatization): 99.32% test accuracy
Decision Tree: 99.41% test accuracy
Naive Bayes: 92.49% test accuracy


Key Findings:

Most models achieved >98% accuracy
Top predictive words for real news: "reuters", "say", "washington"
Top predictive words for fake news: "image", "just", "don't"
Computation time varies significantly between models (SVM: 1676s vs. Logistic Regression: 44s)


Performance-Time Tradeoff:

Logistic Regression offers the best balance of accuracy and computational efficiency
SVM provides highest accuracy but requires significantly more processing time
Lemmatization improves accuracy but adds considerable preprocessing time (672.52s)

#### Next steps
Model Improvement:

Experiment with deep learning approaches such as  Neural Network
Combining strengths of different models (Ensemble methods)



#### Outline of project

- Link to Notebook - https://github.com/udayshankark/CapStone/blob/master/CapStone_NOV16.ipynb

- Link to Project Summary - https://github.com/udayshankark/CapStone/blob/master/ProjectSummary.pdf



##### Contact and Further Information
Uday Kemburu
udayshankark@gmail.com
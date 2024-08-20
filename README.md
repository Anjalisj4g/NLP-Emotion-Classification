# NLP Emotion Classification

**Objective** 


Develop machine learning models to classify emotions in text samples.

Models used :
* Naive Bayes
* Support Vector Machine

Dataset:

https://drive.google.com/file/d/1HWczIICsMpaL8EJyu48ZvRFcXx3_pcnb/view?usp=drive_link

# 1. Loading and Preprocessing

![image](https://github.com/user-attachments/assets/bb06d094-feed-463f-bf0b-cea7d6471b43)

* There are 5937 rows and 2 columns in the dataset.
* There are no missing values in the dataset.
* There are two columns : Comment and Emotion.

## Text Cleaning

* Removed punctuation and numbers.

![image](https://github.com/user-attachments/assets/0e944c1a-31af-4c29-8f83-955c7c24641a)

* Converted to lower case

![image](https://github.com/user-attachments/assets/06460e62-a3fe-42ec-870e-d0c797778733)

## Tokenization

Tokenization is the process of breaking down a piece of text into smaller units called "tokens." These tokens can be words, phrases, or even individual characters, depending on the level of granularity desired. Tokenization is a crucial step in text preprocessing, especially in natural language processing (NLP) tasks, as it transforms text into a format that can be more easily analyzed and processed by machine learning models.

## Stopwords removal

Stopword removal is the process of eliminating common words from a text that are often considered unimportant for certain natural language processing (NLP) tasks. These words, known as "stopwords," include frequently used words. It reduce noises, improve efficiency and enhance model performance.

# 2. Feature Extraction

Feature extraction is the process of transforming raw data into a set of features that can be effectively used by machine learning models. The goal is to capture the most important information in the data while reducing its complexity, making it easier for algorithms to process and learn from the data. In this model, we are using **TfidfVectorizer**.

# 3. Model Development

**Naive Bayes**

* Naive Bayes is easy to implement and understand.
* Naive Bayes performs well with high-dimensional data.
* It is particularly effective with discrete features, making it a natural choice for text classification.
* It requires less preprocessing of data compared to other algorithms.

**Support Vector Machine**

* SVM is a powerful supervised learning algorithm used primarily for classification tasks.
* Effective in Binary and Multiclass Classification.
* SVM tends to be less prone to overfitting.
* It is based on solid mathematical principles of optimization, ensuring reliable performance and predictability.

# 4. Model Comparison

![image](https://github.com/user-attachments/assets/2678dc0a-59b1-4461-b447-a83f75418025)

**Accuracy of Support vector machine(94.61%) is more than that of Naive Bayes(91.33%). Similarly, F1 score of Support vector machine(94.6%) is more than that of Naive bayes(91.33%). Hence, best model is Support vector machine.**



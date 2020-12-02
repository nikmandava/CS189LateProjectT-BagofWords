# CS189LateProjectT-BagofWords
## Learning Objectives
#### Prereqs (16A, 61A, and concurrent week 16B, 61B):
- Vectors
- Svm, logistic regression
- K means clustering
- Basic python and numpy usage
- Features and multiclass classification
- Exposure to computational photography/imaging
- Exposure to the idea of validation
#### Objectives: after completing our assignment, students should be able to:
- Understand what bag of words, and simple NLP problems are
- Implement bag of words in Python
- Implement various adjustments to standard bag-of-words (binary, negative)  to improve model performance
- Apply bag of words to a sentiment analysis problem 
- Be able to use effecient data cleaning for the bag of words model
- Apply the bag of words model to various different training methods students have learned
- Apply basic knowledge of computational imaging to apply bag of words to image classification
- Use previous exposure to featurization and multiclass classification from 16A and 61A and expand on this understanding in bag-of-words featurization
- Use previous exposure to the idea of validation in 16A and 61A to train a model and improve test accuracy

## Intro / Setup
- Notes and slidedeck will give students a base level of understanding on bag-of-words, nlp, and text and image classification. 
- Students will then apply their knowledge by running through each of the project problems in the github repo in numerical order.
- The quiz and quiz solutions can be found in the `quiz` folder
- The blank coding assignments are located in the `Coding_Assignment` folder and the corresponding solutions are located in the `Coding_Assignment_Solution` folder. The data and anything needed for each question is contained within the folder for that question.
   1. `Coding_Assignment/prob1` - Use various bag-of-words featurizations to classify positive/negative Yelp reviews as well as Airline Tweets
       * Students are introduced to sentiment analysis, a common NLP problem
       * Students perform exploratory data anlysis to become familiar with the datasets and learn what kind of words are most associated with positive/negative 
       * Students construct a rudimentary baseline model to compare against
       * Students implement bag of words featurization and train a Logistic Regression model for classification
       * Students implement binary and negative versions of bag of words in order to compare model performance with the standard version 
       * Students examine the trained model to see which words have positive/negative associations
       * Students are presented with an open-ended challenge to improve model accuracy allowing them to used the skills learned in the previous parts
   2. Problem 2 - `SVMAssignment.ipynb`
       * Use bag of words and experiment with data cleaning with an SVM to classify movie reviews from IMDB
   3. Problem 3 - `Image Bag of Words.ipynb`
       * Generate an image vocabulary and then use bag of words with k-means and then an SVM to classify images from the CIFAR-10 dataset

## Installation
* Each of the notebooks uses various common libraries, just `pip install` them 
* Data sets can be downloaded and explored through steps in the notebooks
* For the image classification problem, you may run into version issues with Tensorflow
  * Upgrade tensorflow by running the `pip install --upgrade tensorflow` command in problem 3 notebook

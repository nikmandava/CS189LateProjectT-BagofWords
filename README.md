# CS189 Late Project T- Bag of Words
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
   1. Problem 1 - `Coding_Assignment/prob1` 
       * Use various bag-of-words featurizations to classify positive/negative Yelp reviews and Airline Tweets
       * Students are introduced to sentiment analysis, a common NLP problem
       * Students perform exploratory data anlysis to become familiar with the datasets and learn what kind of words are most associated with positive/negative 
       * Students construct a rudimentary baseline model to compare against
       * Students implement bag of words featurization and train a Logistic Regression model for classification
       * Students implement binary and negative versions of bag of words in order to compare model performance with the standard version 
       * Students examine the trained model to see which words have positive/negative associations
       * Students are presented with an open-ended challenge to improve model accuracy allowing them to used the skills learned in the previous parts
   2. Problem 2 - `Coding_Assignment/prob2` 
       * Use bag of words and experiment with data cleaning with an SVM to classify movie reviews from IMDB
       * The problem begins with asking students to clean data to increase the quality of the vocabulary. Stop words, words without meaning, and punctuation are all removed from the vocabulary. This is included because it is important for the student to understand how to create a strong vocabulary, the linchpin of any good bag-of-words model.
       * Students are asked to observe unclean data to expose how this data is diluted with words that do not add much value to the model.
       * Students are asked to implement and run functions that help create the model so they can learn how to incorporate the features made in bag-of-words into the model itself, and the generation of train and test data.
       * Students are told to fit and test an SVM model that they begin to create in the previous step and are asked to report on the accuracy of the model. This is to make sure students understand how to fit and predict using a SVM classifier, as well as how to interpret the results of the model on data that has not been cleaned yet.
       * Students are finally asked to repeat similar steps, but now with cleaned data. This is so students can compare how the clean data model performs against data that is not cleaned. Students then report and explain their results to test their understanding on how cleaning up a vocabulary affects the model’s accuracy.

   3. Problem 3 - `Coding_Assignment/prob3` 
       * Generate an image vocabulary and then use bag of words with k-means and then an SVM to classify images from the CIFAR-10 dataset
       * First students are asked to load and clean data to train and test on and to comment on the data to get them thinking about how features can be extracted from an image.
       * Next students are asked to complete a function where they use pysift to detect keypoints in an image and extract features from it. This function returns train and test image data. This part of the problem helps students learn how to define an image by a set of smaller parts of the image, similar to words in bag-of-words.
       * Students are asked to create a vocabulary from the image features, which will be used in the bag-of-words feature model in the coming steps. This shows similarity between image and text classification.
       * Students are asked to perform bag-of-words on the image features to return a ready to use training set of features to help them learn how to perform classification on an image and fully featurize the image.
       * In the last parts of the problem, the student is asked to train and test an SVM classifier and report on the results. This part ensures that students understand the goals of the assignment and reflect on the performance of bag-of-words for image classification. In addition, we ask the student to perform hyperparameter tuning so that they are able to see how different parameters affect the vocabulary and ultimately the whole image classification model.
## Navigating the Repository
* Notes and slides are located in the `content` folder
* The quiz questions and solutions can be found in the `quiz` folder
* The blank coding assignments are located in the `Coding_Assignment` folder and the corresponding solutions are located in the `Coding_Assignment_Solution` folder. The data and anything needed for each question is contained within the folder for that question.
## Installation
* Each of the notebooks uses various common libraries; if any library is not included, use `pip install` to install them 
* Data sets can be downloaded and explored through steps in the notebooks
* For the image classification problem, you may run into version issues with Tensorflow
  * Upgrade tensorflow by running the `pip install --upgrade tensorflow` command in problem 3 notebook

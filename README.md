# Quora Question Pair Similarity

### Source: https://www.kaggle.com/c/quora-question-pairs 

## Business Problem
Over 100 million people visit Quora every month, so it's no surprise that many people ask similarly worded questions. Multiple questions with the same intent can cause seekers to spend more time finding the best answer to their question, and make writers feel they need to answer multiple versions of the same question. Quora values canonical questions because they provide a better experience to active seekers and writers, and offer more value to both of these groups in the long term.

Currently, Quora uses a Random Forest model to identify duplicate questions. In this competition, Kagglers are challenged to tackle this natural language processing problem by applying advanced techniques to classify whether question pairs are duplicates or not. Doing so will make it easier to find high quality answers to questions resulting in an improved experience for Quora writers, seekers, and readers.

## Problem Statement
Identify which questions asked on Quora are duplicates of questions that have already been asked.   
This could be useful to instantly provide answers to questions that have already been answered.  
We are tasked with predicting whether a pair of questions are duplicates or not. 

## Business Objectives and Constraints
1. The cost of a mis-classification can be very high.  
2. You would want a probability of a pair of questions to be duplicates so that you can choose any threshold of choice.  
3. No strict latency concerns.  
4. Interpretability is partially important.

## Data Overview
- Data will be in a file Train.csv  
- Train.csv contains 5 columns : qid1, qid2, question1, question2, is_duplicate  
- Size of Train.csv - 60MB  
- Number of rows in Train.csv = 404,290 

## Machine Leaning Problem
A binary classification problem, for a given pair of questions we need to predict if they are duplicate or not.

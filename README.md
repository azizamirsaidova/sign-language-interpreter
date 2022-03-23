# LeapmotionMLProject

# Task Proposed:
● We plan to build a model to translate hand gestures into spoken language, English

● Sign Language is one of the commonly used languages in the USA (Ref 1)

● Sign Language is one of the languages that is hard to understand for spoken language
users without training. Even though it is used by approximately 0.25 million to 0.50
million people in the USA(Ref 2), sign language is considered challenging to learn

● This can be shown by the employment gap of 22.5% between the deaf and hearing
populations (Ref 3)

● Building a tool for individuals to translate sign language into spoken language would add
a lot of value for the sign language users to narrow the employment gap between Sign
Language users and Spoken Language users

● Sign language translation can also help the 0.6 million deaf individuals who require
mental treatment every year (Ref 5)

https://user-images.githubusercontent.com/90999624/149116872-f8351646-8405-4b94-a720-b631fd14d60c.mp4


# Data Source:
We are planning to use the data from Kaggle using Leap Motion Sensors(Ref 4) which
captures hand gestures images and converts them to various dimensions
The following shows the basic dimensions of the data

● Data Set: ASL-leap-motion.csv | BSL-leap-motion.csv

● No. of Rows: 5,146 | 16,498

● No. of Independent Columns: 428

● No. of Dependant Columns: 1

● Dependant Column: Labelled data with words represented by the respective columns

● Independent Columns Examples: Left Hand Direction, Right Wrist Position, Left Thumb
Proximal start, etc.


# Attributes:
We want to use these in the data set from Ref 4 and create hypotheses to evaluate if they
are useful and proceed with using the relevant ones. We have 428 dimensions in total in our
dataset. We understand their distributions and perform any treatments necessary. Perform
exploratory data analysis and proceed to build our hypotheses. Evaluating our hypotheses we
will build a model which can convert these signals to text.

4.1 Methods Proposed:
We plan to do this project in 5 steps where our work comes in a couple of steps.
However, depending on the feasibility we might be modifying the project which will be
elaborated further.
Fig 1. The Proposed Schema of the End-to-End Solution

4.2 Approach:
We plan to build a model using the data from Kaggle’s Leap Motion sensor. The
modeling approach is to create a classification model to classify the gestures data to a specific
word. These words can be organized to form sentences leveraging the 18 words in the datasets.
As for the final demonstration, we plan to use the leap motion sensor to convert sign
language into sentences. If this seems not feasible, we will just showcase our success through the
success metrics mentioned below.

4.3 Data-Preprocessing:
We plan to check the columns for any anomalies between specific classes and try to
evaluate why those occurred and treat them, if necessary. Additionally, we will check for missing
values to treat them accordingly.
Furthermore, we will start by understanding the distributions of the various dimensions
q to remove any multicollinearity, by using factor analysis, PCA or basic transformations. We
plan not to drop any columns completely unless they are represented in one way or another by
another set of columns.
Proposed ML Techniques:
The problem we are working on is a Classification problem so we plan to work with
techniques such as Naive Bayes, Hidden Markov Models, Neural Networks, Decision Trees,
K-nearest Neighbors.
Success Metrics:
To measure the performance of the classification model, we plan to utilize sum the
following metrics to evaluate our model:

● Accuracy

● Precision

● F-1 Score

● Sensitivity

● Specificity

● MCC (Matthew's Correlation Coefficient)

So, as our model would be a multi-class classification system, these metrics need to be modified
accordingly. Creating these metrics, we will build a model focusing on providing outputs of
classes from 0-16 and generate these metrics. Based on these metrics we will tune the
hyperparameters and retrain our model.

[MSAI349 - ASL Translation.pptx](https://github.com/saumyasingh98/LeapmotionMLProject/files/7853528/MSAI349.-.ASL.Translation.pptx)


# References:
1. https://en.wikipedia.org/wiki/Languages_of_the_United_States
2. https://www.gallaudet.edu/documents/Research-Support-and-International-Affairs/ASLUsers.pdf
3. https://www.nationaldeafcenter.org/sites/default/files/Deaf%20People%20and%20Employment%20in%20the%20United%20States_%202019%20(7.26.19)(ENGLISH)(WEB).pdf
4. https://www.kaggle.com/birdy654/sign-language-recognition-leap-motion
5. https://www.gallaudet.edu/office-of-international-affairs/demographics/deaf-employment-reports/


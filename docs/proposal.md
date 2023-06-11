# Draft Proposal

- **Author:** Mindy Wang
- **Term:** Summer 2023
- **Title:** Predicting injury due to malfuction of medical device
- ***Feature:*** Event text
- ***Target:*** injury or not (a derived field from event type)

>The issue of interest is to find out what kinds of malfunction cause patient injury from the event text. It is important to find out what kind of malfunction can cause injury so we can focus more on how to prevent them from happening to save patients from suffering.
I want to know if there are a few topics (issues) that are most mentioned in event text.  I also want to do train/test split and use event text to predict patient injury.
The data is from FDA, which has its credibility just because it is from a credible source.  There is some data that appear to be not conforming with the column name. However, overall, the data quality is good. There are 500 records of the data, and which covered the adverse event spreading between Jan 1, 2020 and May 31, 2023.
My unit of study will be each event reported. There are 500 records.
The target variable is injured or not.  The feature is event text. 
I will clean the data and do necessary preprocessing to come up with text that can be used for analysis. I planned on using use Multinomial Naive Bayes classifier to do the NLP analysis. I will use run confusion matrix and calculate accuracy scores to evaluate how well the model performs.
I hope to be able to contribute to the discovery of what kinds of medical device malfunction will cause injury, therefore we can find out what we can do to prevent those kinds of malfunction from happening. Currently I don’t have a clear idea of what I can deploy the trained model yet.


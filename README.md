# Mindy_Data606
## Date Source: From open FDA.  MAUDE - Manufacturer and User Facility Device Experience https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfmaude/results.cfm

I download 500 records reported from 01/01/2020 to 05/31/2023

## The results of preliminary EDA:
There are mostly malfunctions without patient injury.  I identified 10 products what reported the most adverse event and used a bar chart to display the results.  I identified the top 10 patient problems and used a bar chart to display the results.  I identified the top 10 manufacturers that reported the most adverse events and used a bar chart to display it.

## Research question:  
I intend to do an NLP study on Adverse Events reported on medical devices to FDA.  I will use Multinomial Naive Bayes classifier to do the analysis.  There is a variable called event text.  I would like to use it to predict whether the patient is injured or not.  I hope to be able to contribute to the discovery of the causes of injury due to medical device malfunction.
I will do data cleaning first.  I will change the text to lower case since it is all upper case now and tokenize the data.  I will remove stop words and add “Event Description:” to the stop words dictionary.  
I might also do topic modeling to find out if there are some common topics in these event descriptions.  Then, I will use Multinomial Naive Bayes classifier to do the analysis.  There is a variable called event text.  I would like to use it to predict whether the patient is injured or not.  I hope to be able to contribute to the discovery of the causes of injury due to medical device malfunction.
### Feature: Event text
### Target: injury or not (a derived field from event type)


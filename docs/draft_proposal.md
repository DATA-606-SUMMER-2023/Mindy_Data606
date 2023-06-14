# Draft Proposal

- **Author:** Mindy Wang
- **Term:** Summer 2023
- **Title:** Predicting injury due to malfuction of medical device
### Introduction:
The purpose of this proposal is to outline a data science project focused on predicting patient injury due to medical device malfunction using NLP techniques. The dataset was sourced from the open FDA MAUDE (Manufacturer and User Facility Device Experience) database, specifically the adverse event reports related to medical devices. By analyzing the event text and using a Multinomial Naive Bayes classifier, the goal is to contribute to the discovery of the causes of injury and improve patient safety.
### Research Question:
The primary research question for this project is:
Can we predict whether a patient is injured or not based on the event text reported in adverse event records related to medical device malfunction?
### Data Description:
- **Data Source:** The data were collected from the open FDA MAUDE database, available at https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfmaude/results.cfm.
- **Data Collection:** A total of 500 records was downloaded, covering the period from January 1, 2020, to May 31, 2023.
- **Data Credibility:** The dataset is from a credible source open FDA.
- **Data Quality:** Even though there are a few data that appear to be not conforming with the column name, overall, the data quality is very good. 
- **Unit of Study:** My unit of study will be each event reported. 
- **Feature:** My feature will be event text.
- **Target:** My target for prediction will be injured or not (a derived field from event type)
-**Preliminary EDA:** Initial exploratory data analysis revealed that most reported adverse events are malfunctions without patient injury. The top 10 products, top 10 patient problems, and top 10 manufacturers reporting adverse events were identified and visualized using bar charts. Those findings and bar charts are presented in the EDA notebooks.
### Methodology:
- **Data Cleaning:** The first step will involve data cleaning, including converting the event text to lowercase, remove special characters and puctuations, and lamitization or steming, tokenizing the data, and removing stop words. Additionally, the phrase "Event Description:" will be added to the stop words dictionary to remove it from the text.
- **Classification Model:** A Multinomial Naive Bayes classifier will be trained using the cleaned event text as the feature and the derived field of injury or not as the target variable. The dataset will be split into training and testing sets to evaluate the model's performance accurately.
- **Evaluation:** The model's performance will be assessed using metrics such as accuracy, precision, recall, and F1 score. A confusion matrix will also be generated to understand the model's predictions in more detail.
- **Topic Modeling:** After the above are done, if time permits, topic modeling techniques, such as Latent Dirichlet Allocation (LDA), will be applied to identify common topics within the event descriptions. This will provide insights into recurring issues related to medical device malfunctions.
### Expected Outcomes: 
The project aims to contribute to the discovery of the causes of injury due to medical device malfunction by predicting patient injury based on the event text reported in adverse event records. The expected outcomes include:
•	Evaluation of the Multinomial Naive Bayes classifier's performance in predicting patient injury.
•	Insights into the types of malfunctions that are more likely to cause patient injury.
•	Potential recommendations for preventing or mitigating the identified malfunctions to improve patient safety.
•	Identification of common topics or issues mentioned in the event descriptions.
### Conclusion: 
This data science project will focus on analyzing adverse event reports related to medical device malfunction using NLP techniques. By predicting patient injury based on the event text, the aim is to contribute to the discovery of the causes of injury and enhance patient safety. The project will involve data cleaning and training a Multinomial Naive Bayes classifier. The performance of the model will be evaluated, and recommendations for preventing injuries caused by medical device malfunction will be provided based on the findings. If after the prediction was made, a topic modeling of the event text may be added if time permits. Additional data may be downloaded if needed.


# Predicting injury due to malfunction of medical device 
### my Youtube video: https://youtu.be/WK11pJSLpKs
### my power point presentation: https://github.com/ymindywang/Mindy_Data606/blob/main/docs/Capston_NLP_Mindy%20Wang.pptx
### my Github repo: https://github.com/ymindywang/Mindy_Data606
- **Author:** Mindy Wang
- **Term:** Summer 2023
- **Title:** Predicting injury due to malfunction of medical device
## Introduction:
The purpose of this proposal is to outline a data science project focused on predicting patient injury due to medical device malfunction using NLP techniques. The dataset was sourced from the open FDA MAUDE (Manufacturer and User Facility Device Experience) database, specifically the adverse event reports related to medical devices. By analyzing the event text and using a Multinomial Naive Bayes classifier, the goal is to contribute to the discovery of the causes of injury and improve patient safety and prevent future injury.
## Research Question:
The primary research question for this project is:
Can we predict whether a patient is injured or not based on the event text reported in adverse event records related to medical device malfunction?
## Data Description:
- **Data Source:** The data were collected from the open FDA MAUDE database, available at https://www.accessdata.fda.gov/scripts/cdrh/cfdocs/cfmaude/results.cfm.
- **Data Collection:** A total of 500 records was downloaded, covering the period from January 1, 2020, to May 31, 2023.
- **Data Credibility:** The dataset is from a credible source open FDA.
- **Data Quality:** Even though there are a few data that appear to be not conforming with the column name, overall, the data quality is very good. 
- **Unit of Study:** My unit of study is each event reported. 
- **Feature:** My feature is event text.
- **Target:** My target for prediction is injured or not (a derived field from event type)
## Background:
In this study, a dataset of adverse event (AE) reports was utilized to develop a predictive model for determining whether malfunctions result in injury. The dataset was divided into training and testing subsets with an 80/20 split ratio. The goal was to leverage natural language processing (NLP) techniques to analyze the text within AE reports and predict the occurrence of injuries. The dependent variable in this analysis was the presence or absence of injury, while the independent variable was the text content of the AE report.
## Preliminary EDA:
Prior to modeling, exploratory data analysis (EDA) was conducted to gain insights into the dataset's characteristics. Initial exploratory data analysis revealed that most reported adverse events are malfunctions without patient injury. The top 10 products, top 10 patient problems, and top 10 manufacturers reporting adverse events were identified and visualized using bar charts. Those findings and bar charts are presented in the EDA notebooks and the power point presentation.
## Methodology:
- **Data Cleaning:** To prepare the text data for analysis, a series of preprocessing steps were applied. The first step involves data cleaning, including converting the event text to lowercase, remove special characters and punctuation, and lemmatization, tokenizing the data, and removing stop words. Additionally, the phrase "Event Description:" was added to the stop words dictionary to remove it from the text.
- **Classification Model:** A Multinomial Naive Bayes classifier was trained using the cleaned event text as the feature and the derived field of injury or not as the target variable. The dataset was divided into training and testing subsets with an 80/20 split ratio to evaluate the model's performance accurately. 
- **Evaluation:** The model's performance was assessed using metrics such as accuracy, precision, recall. A confusion matrix was generated to understand the model's predictions in more detail.
## Expected Outcomes: 
The project aims to contribute to the discovery of the causes of injury due to medical device malfunction by predicting patient injury based on the event text reported in adverse event records. The expected outcomes include:
- Evaluation of the Multinomial Naive Bayes classifier's performance in predicting patient injury.
- Insights into the types of malfunctions that are more likely to cause patient injury.
- Potential recommendations for preventing or mitigating the identified malfunctions to improve patient safety.
- Identification of common topics or issues mentioned in the event descriptions.
## Results:
Multinomial Naive Bayes (NB) algorithm was employed to predict whether an injury occurred based on the AE report text. The model's accuracy, precision, and recall were evaluated as part of the performance assessment. The achieved results demonstrated promising performance: an accuracy of 0.86, precision of 0.87, and recall of 0.86. Given the relatively small number of records in this study.  The model’s performance is very good. Furthermore, a word count was generated for both visualization purposes and the creation of a word cloud, which visually represented the most frequent words in the text. The analysis revealed that certain words such as "report," "patient," "device," and "implant" frequently appeared in the context of injury-related reports.
## Future Research Direction: 
In future research, the study aims to enhance its predictive capabilities by incorporating topic modeling techniques. Topic modeling will enable the identification of recurring themes or topics within the AE report text, potentially uncovering patterns that contribute to the prediction of injuries. This analytical approach could provide valuable insights into the underlying causes and factors associated with adverse events.
The study acknowledges certain limitations. The dataset comprised only 500 records, which, despite yielding promising results, might not fully capture the complexity of real-world scenarios. As such, future endeavors will involve expanding the dataset to assess if increased data volume translates to improved accuracy. 
## What the Author Has Tried:
The author has tried to augment the stop word list with common words that might not contribute significantly to injury prediction, to investigate if this refinement enhances the model's performance. However, the model accuracy decreased slightly as a result of the modification.  Therefore, the author decided to revert back to the original stop word list.   The reason may be that when the patient is injured due the malfunction of the medical device, the AE report mentioned words such as "report," "patient," "device," and "implant" more often than when the patient is not injured.
## Conclusion: 
In conclusion, this study leveraged NLP techniques and the Multinomial NB algorithm to predict injuries resulting from malfunctions based on AE report text. The obtained accuracy, precision, and recall metrics demonstrated the potential of this approach. Future investigations will incorporate topic modeling techniques, such as Latent Dirichlet Allocation (LDA) to identify common topics within the event descriptions. This will provide insights into recurring issues related to medical device malfunctions.  In addition, the author will refine the analysis with an expanded dataset. The study aims to advance its predictive capabilities and provide more nuanced insights into adverse event outcomes and hopefully that will help with future prevention of patient injury due to medical device malfunction.
## References:
- Wang, L. et. al. (2022). Assessment of electronic health record for cancer research and patient care through a scoping review of cancer natural language processing. JCO Clinical Cancer Informatics 6.
https://ascopubs.org/doi/full/10.1200/CCI.22.00006
- Ariwala, P. (Jun 15, 2023). Top 14 Use Cases of Natural Language Processing in Healthcare. Maruti Techlabs. https://marutitech.com/use-cases-of-natural-language-processing-in-healthcare/
- Ariwala, P. (Apr 3, 2023). Unlocking the Power of NLP in Healthcare: A Comprehensive Review. Maruti Techlabs. https://marutitech.com/nlp-in-healthcare/






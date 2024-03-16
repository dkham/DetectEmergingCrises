# DetectEmergingCrises

![Disaster-Relief-page-banner](https://github.com/dkham/dkham/assets/72950291/125f58c1-7a95-44d2-b07e-7f2acc9c61af)

**Problem and Motivation**

Humanitarian organizations need actionable information to effectively launch relief efforts to disaster areas. Social media platforms, like Twitter, have become an important information source for crisis management. Humanitarian organizations can use Tweets to identify emerging disasters, but they struggle to parse through large amounts of data. With our application, we hope to promptly summarize critical information to aid organizations in mitigating crisis situations. 

**Data Source and Data Science Approach:**

For this project, we use multi-class and multi-label classification models to:

Identify disaster tweets by disaster event
Identify disaster tweets by disaster type (e.g. hurricane, flood, etc.);
Categorize the type of disaster information (e.g. news, emerging threat); and
Categorize tweets by priority level.
We use a database acquired from TREC-IS that is comprised of multiple Twitter datasets collected from a range of past wildfire, earthquake, flood, hurricane, bombing and shooting events. Each tweet is assigned a 'priority' label, that indicates how critical the information within that tweet is. In addition, TREC-IS includes 25 information type labels that have been manually assigned by human annotators, such as 'contains location' or is a 'search and rescue request'. In total, the TREC-IS we are using has manually annotated tweet streams for 42 emergency events, comprising over 40,459 labelled tweets.

**Evaluation**

To evaluate our models, we use accuracy scores, classification reports, and confusion matrices to understand the performance of our classification models. 

**Key Learning & Impact**

We set out to find the best model for our classification task using approaches that we found were effective from academic papers. We compared and tested models that included: LinearSVC, Multinomial Logistic Regression, MultinomialNB, and Random Forest. While a simplistic model, we found LinearSVC consistently outperformed the others. This may be due to Support Vector Machines (SVMs) performing well with clear separation of classes, of which our dataset has. We also learned the importance of balancing datasets to ensure accurate predictions. We applied RandomOversampler to our imbalanced dataset which supplements the training data with multiple copies of some of the minority classes. 


![disaster_management_dashboard_showing_risk_consequences_type_location_ppt_powerpoint_master_slide_slide01](https://github.com/dkham/dkham/assets/72950291/a5e15c3f-d895-417e-aff7-e35b1500a3c7)


**Acknowledgements**

We are grateful to have the guidance and encouragements from our Capstone Advisors, Dr. Frederick Nugen and Dr. Puya H. Vahabi, of the Master of Information and Data Science program at the School of Information, University of California, Berkeley.

Daisy &amp; Nathan's Capstone Project Summer '23

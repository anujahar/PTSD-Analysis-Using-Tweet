# PTSD-Analysis-Using-Tweet

**Motive:**
Post Traumatic Stress Disorder [PTSD] is a psychiatric disorder that can occur in people who have experienced or witnessed a traumatic event such as assault, war or a natural disaster. People with PTSD have intense, disturbing emotions related to their trauma, and left undiagnosed can lead to anxiety, depression and other harming thoughts. According to the National Institute of Mental Health, 1 in 13 adults develop PTSD and about 50% of them don’t seek professional help. Recent research work has shown the utility of social media data for studying PTSD, a more efficient approach than relying on collecting information from healthcare professionals.
 
**Objective:**
Through our analysis, we aimed to identify distinct topics among the tweets by people with PTSD, 6 months pre and post their diagnosis date. Further, we built and trained two predictive models to correctly classify whether or not a person has PTSD based on their Twitter behavior.

**Method:**
We conducted a study on 43 twitter users who were clinically diagnosed with PTSD to determine if there was any change in their tweets before and after their PTSD diagnosis. We curated a dataset by obtaining tweets 6 months prior and post the PTSD diagnosis date for the users. We used topic modelling using semi supervised LDA to determine any key changes in the topics identified with the help of keywords before and after the user’s diagnosis date.
Further, we built an additional dataset of 72 twitter users who were clinically diagnosed with PTSD however the diagnosis date information was not available via their tweets. We added a control group of 46 users with a Matched Pair approach to balance our dataset. We obtained a total 139040 tweets of all the 118 users in our dataset and divided the dataset into train and test data keeping in mind the balance of the ratio of users diagnosed with PTSD and control group in both. We built Logistic Regression and Support Vector Classifier [SVM] models to predict users diagnosed with PTSD based on their tweets.

**Results:**
After performing semi-supervised topic modeling using anchor words on the pre and post diagnosis date datasets, we obtained four distinct topics for each. For the pre diagnosis dataset, we found causes, feelings and emotions, physical symptoms, and mental symptoms. For the post diagnosis datasets, our topics were symptoms, feelings and emotions, therapy and support, and coping mechanisms. We then moved on two building two binary classifiers: Logistic Regression and Linear Support Vector Machine. Our models correctly classified whether or not a user has PTSD with an accuracy of 52% and 78% respectively. 

**Conclusions:**
Although we were able to achieve our goals of identifying distinct topic models between pre and post diagnosis datasets as well as build classifiers to predict whether or not a person has PTSD, our analysis was performed at a classroom level, with limited access to web scraping tools. This research can be scaled to incorporate other social media platforms such as Facebook and Instagram as well as focus on a user’s overall social media profile (number of likes, shares, videos, profile pictures etc.) to reach more insightful conclusions. 





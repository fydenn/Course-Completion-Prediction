# Course Completion Prediction
Online learning platforms face a critical challenge: a high percentage of users abandon courses before completion. For providers, this leads to lost revenue (especially for paid courses or post-completion monetization), inefficient marketing spend (on users unlikely to finish), and reputational risks (due to poor learner experiences). Without understanding why users drop out, companies struggle to retain at-risk learners, optimize course content, or forecast revenue accurately—resulting in missed growth opportunities.

My goal is Develop an ML model to predict dropout probability based on behavioral data (engagement time, progress), enabling:

- Targeted interventions: Automated nudges/support for high-risk users.

- Curriculum improvements: Identify and fix pain points in courses.

# Technologies
- RandomForestClassifier
- GridSearchCV
- Pandas
- NumPy
- Matplotlib
- seaborn

# EDA
Number of unique users by date:

![Image](https://github.com/user-attachments/assets/7691e43a-dfc3-463c-aba6-40eeff757154)

Actions depending on the time of day:

![Image](https://github.com/user-attachments/assets/2ddae2b8-77e0-4921-a9c3-215d25914ebd)

Difference between 2 lasts entring of every user:

![Image](https://github.com/user-attachments/assets/40a356a0-cc76-4a22-8f53-2c4598b5e77f)

Complited tasks by user:

![Image](https://github.com/user-attachments/assets/6c2dc2ed-833b-46fd-8609-29e9d97a3bc4)


# Prediction using Machine learning
Metrics for machine learning solution: Pressicion. I chose this metric because it is very important for us to accurately predict whether a user will leave our platform in order to avoid spending more money.

For this case i chose the RandomForestClassifier because it has the advantage of being flexible in terms of data fit, but is less prone to overfitting.
using GridSearchCV I got the following hyperparameters : 
- 'max_depth' = 6,
- 'min_samples_split' = 120,
- 'n_estimators' = 13

Most important Features:

![Image](https://github.com/user-attachments/assets/0d98eb97-b7b2-4cee-a927-0281b4cd745f)

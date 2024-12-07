# MSBA-Capstone-Fall-2024
 

Swire Coca-Cola Machine Downtime Prediction Capstone
Business Problem:
Swire Coca-Cola faces significant operational challenges due to unplanned machine downtimes, leading to an estimated $60 million in annual losses. These disruptions affect production efficiency and increase operational costs. Addressing this issue is critical for ensuring uninterrupted production and minimizing revenue losses.

Project Objective:
The goal of this project was to develop predictive models capable of identifying key drivers of machine downtimes and accurately predicting major breakdowns. By leveraging data analytics and machine learning, I aimed to deliver actionable insights that enable Swire Coca-Cola to proactively manage machine maintenance and improve operational efficiency.

Solution:
I used a combination of Exploratory Data Analysis (EDA) and machine learning to analyze downtime data and predict breakdown risks. Key components of the group solution include:

Random Forest Model: Achieved an Out-of-Bag error rate of 6.93% and an accuracy of 89.59%, effectively identifying high-risk machines and critical downtime predictors.
Feature Engineering: Introduced key variables such as machine age, minor vs. major breakdown classification, and rolling average downtime trends to enhance predictive power.
Insights: Highlighted the importance of frequent minor breakdowns as a leading indicator of major breakdowns and emphasized the role of machine age in planned maintenance.

Key Findings:

Breakdown Classification:

Machines with frequent minor breakdowns (<60 minutes) are more likely to experience major breakdowns (>60 minutes).
Machine age was found to be a significant predictor, with newer equipment requiring more planned maintenance.

Feature Importance:

Maintenance-related features such as maintenance plans and order descriptions were among the most critical in predicting major breakdowns.

Cost Impact:

Reducing major breakdowns by 20% could save Swire Coca-Cola approximately $3.8 million annually.
Files in Repository:

EDA.RMD: My personal EDA file contributing to the group's EDA
FINAL_MODELING.RMD: My personal Modeling file contributing to the group's modeling phase. 
Modeling GROUP.RMD: Our group notebook delivered to the project sponsor.

Contributions:

In this project, I independently:
-Conducted EDA to analyze downtime patterns, identify data quality issues, and visualize trends.
-Built and optimized an XGBoost to predict breakdowns. I ultimately wasn't able to successfully get it to run, but my data preparation assisted with my group members' models
-Designed new variables, such as failure risk categories and rolling average downtimes, to improve model performance.
-Synthesized findings into actionable recommendations for Swire Coca-Cola.
-Assisted greatly with the compilation of .RMD files containing our findings

Business Value:

Proactive Maintenance Planning: The insights enable Swire Coca-Cola to identify high-risk machines and schedule maintenance before major breakdowns occur.
Cost Savings: The models provide a roadmap for reducing downtime-related losses by millions annually.
Improved Data Processes: Highlighting the need for improved data tracking (e.g., machine age) to enhance future analyses.
Difficulties Encountered:
One of the main challenges was dealing with missing data in critical variables such as machine age and certain equipment-related fields. For instance:

Machine Age Data: The lack of consistent tracking meant that machine age could only be calculated for planned maintenance events. This limited its application as a predictive feature across all data.
Imbalanced Data: Some categories (e.g., minor vs. major breakdowns) had disproportionately large or small sample sizes, complicating model training.
Data Completeness: Many fields had high percentages of missing values, requiring imputation or removal to maintain model quality. Columns with over 80% missing data were ultimately excluded due to their limited value.
These challenges underscored the importance of improving data collection processes for future predictive analytics.

Lessons Learned:

Data Quality Matters: Addressing missing data and feature engineering were critical to the project’s success.
Real-World Data Challenges: Managing imbalanced data and aligning findings with business objectives were key hurdles.

Going through this process, I also learned that it's better to make things simple and build from there. I think we would've been successful had we focused on one or two plants and analyzed their data and then see if our findings made sense for other plants.

Next Steps:

Continue working on the XGBoost model to see if any new results emerge
Implement the Random Forest model into Swire Coca-Cola’s production systems for real-time breakdown monitoring.
Develop processes for tracking and analyzing machine age and downtime trends.
Use insights from minor breakdowns to optimize preventative maintenance strategies.
This project showcases how predictive analytics can transform operational efficiency and drive significant cost savings for Swire Coca-Cola. For more details, refer to the files in this repository.

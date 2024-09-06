# Strikers-performance-analysis
Introduction

In the world of football, strikers play a pivotal role in deciding the fate of matches and championships. Identifying the best strikers among a pool of talent involves a comprehensive analysis of various factors ranging from performance metrics to personal attributes. In this project, titled "Segmenting and Classifying the Best Strikers," we delve into a dataset containing information on 500 strikers, aiming to uncover patterns, insights, and classifications that distinguish top-performing strikers from the rest.

##Project Description
The project involves utilizing data analytics techniques to explore and understand the characteristics and performance metrics of strikers. By employing descriptive statistics, data visualization, feature engineering, and machine learning algorithms, we aim to identify the key attributes that contribute to a striker's success on the field and classify them into different categories based on their performance.

##Purpose
The primary purpose of this project is to provide a systematic framework for analyzing and categorizing strikers based on their performance metrics and personal attributes. By doing so, coaches, scouts, and football analysts can gain valuable insights into the characteristics of top-performing strikers and make informed decisions in team selection, recruitment, and strategic planning.

##Dataset Description
The dataset comprises various variables related to 500 strikers, encompassing both demographic information and performance metrics. Key variables include nationality, footedness, marital status, goals scored, assists, shot accuracy, dribbling success, and many more, providing a comprehensive overview of each striker's profile and on-field performance.

Striker ID: Unique identifiers assigned to each striker.

Nationality: The country of origin for each striker.

Footedness: Indicates whether the striker is right or left-footed.

Marital Status: Indicates whether the striker is married (yes) or unmarried (no).

Goals Scored: The total number of goals scored by the striker, a fundamental performance metric.

Assists: The number of assists provided by the striker, indicating their ability to create goal-scoring opportunities for teammates.

Shots on Target: The number of shots taken by the striker that hit the target, reflecting their ability to create scoring opportunities and test the goalkeeper.

Shot Accuracy: The percentage of shots on target out of total shots taken, showing the striker's precision and effectiveness.

Conversion Rate: The percentage of shots that result in goals, revealing the striker's efficiency in front of goal.

Dribbling Success: A metric indicating the striker's ability to bypass defenders and create goal-scoring opportunities through individual skill.

Movement off the Ball: Reflects how actively the striker moves to find space and create opportunities for themselves and teammates.

Hold-up Play: Measures the striker's ability to retain possession and bring teammates into play with passes or layoffs.

Aerial Duels Won: The number of aerial duels won by the striker, important for strikers strong in the air as it can create scoring chances.

Defensive Contribution: Reflects the striker's defensive efforts such as tracking back, pressing opponents, and making interceptions.

Big Game Performance: Indicates the striker's performance in important matches, which can elevate their reputation.

Consistency: Reflects how regularly the striker performs at a high level over the course of a season or multiple seasons.

Versatility: Measures the striker's ability to adapt to different tactical systems and roles within the team.

Penalty Success Rate: The efficiency of the striker from the penalty spot, crucial in tight matches.

Impact on Team Performance: Reflects how the team's results and overall attacking play are influenced by the striker's presence.

Off-field Conduct: Measures the striker's professionalism, leadership, and behavior, which can impact their overall performance and value to the team.

Required Tools
Python programming language

Jupyter Notebook

Questions to solve
Data Cleaning:

Download the attached dataset and load it into Jupyter notebook.

Load all the relevant and necessary packages for the required tasks.

Check for missing values within any column and use SimpleImputer to impute the missing values. Use strategy 'median' for numeric and 'most frequent' for nominal columns.

Check for the correct data types and assign integer data types for specific variables: 'Goals Scored', 'Assists', 'Shots on Target', 'Movement off the Ball', 'Hold-up Play', 'Aerial Duels Won', 'Defensive Contribution', 'Big Game Performance', 'Impact on Team Performance', 'Off-field Conduct'.

Descriptive Analysis:

Perform descriptive analysis on the dataset. Round the output values by 2 decimal points.

Data Visualization:

Perform percentage analysis on the variable Footedness and create a pie chart on the output using matplotlib.

Visualize the distribution of players' footedness across different nationalities in a countplot of seaborn.

Statistical Analysis:

Determine which nationality strikers have the highest average number of goals scored.

Calculate the average conversion rate for players based on their footedness.

Find whether there is any significant difference in consistency rates among strikers from various nationalities. Before doing the appropriate test, must check for the assumptions.

Check if there is any significant correlation between strikers' Hold-up play and consistency rate. Must check for the assumptions.

Check if strikers' hold-up play significantly influences their consistency rate.

Feature Engineering:

Create a new feature - Total contribution score by summing up specific columns: 'Goals Scored', 'Assists', 'Shots on Target', 'Dribbling Success', 'Aerial Duels Won', 'Defensive Contribution', 'Big Game Performance', 'Consistency'.

Encode the Footedness and marital status by LabelEncoder.

Create dummy variables for Nationality and add them to the data.

Clustering Analysis:

Perform KMeans clustering:

Select features by dropping the Striker_ID from the updated data.

Calculate the Within-Cluster-Sum-of-Squares (WCSS).

Visualize the elbow chart to select the optimal number of clusters (The breakpoint of elbow chart must show 2).

Build the KMeans cluster with the optimal number of clusters and add the labels into the data.

Calculate the average total contribution score by the value of clusters.

Assign the tag 'Best strikers' for 0 and 'Regular strikers' for 1 and add a new column 'Strikers types' into the data. Drop the Clusters variable.

Use feature mapping to map the new feature Strikers types: 'Best strikers' for 1 and 'Regular strikers' for 0.

##Machine Learning Model:

Select the features into x and the target column Strikers types into y. Must delete unnecessary columns (i.e., 'Strikers_ID') while selecting the features.

Perform feature scaling with StandardScaler and split the data into train and test sets where the test data size will be 20%.

Build a logistic regression machine learning model to predict strikers type.

Make predictions and evaluate by calculating the accuracy percentage.

Create the confusion matrix and visualize it.

Finally, answer the question asked in this assignment and you are done!



##Conclusion
Through a comprehensive analysis of the dataset, we've gained valuable insights into the characteristics and performance metrics of strikers. By segmenting and classifying the strikers based on their attributes and performance, we've provided a framework for identifying top-performing strikers and predicting their performance type. This project serves as a valuable resource for football professionals and enthusiasts alike, aiding in talent identification, team selection, and strategic planning.

##Relevant Questions to solve
What is the maximum goal scored by an individual striker?

What is the portion of Right-footed strikers within the dataset?

Which nationality strikers have the highest average number of goals scored?

What is the average conversion rate for left-footed player?

How many left footed players are from France?

What is the correlation co-efficient between hold up play and consistency score?

What is the p-value for the shapiro wilk test of consistency score? Is it normally distributed?

What is the p-value for the levene's test of ANOVA analysis? Is the heteroscedasticity assumed?

Is there any significant correlation between strikers' Hold-up play and consistency rate?

Describe t

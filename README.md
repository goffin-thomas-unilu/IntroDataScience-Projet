# Project Data Science

### As a candidate for the Data Analyst position at the Ministry of Health in Luxembourg, we present you with a comprehensive task that encompasses data exploration, analysis, and predictive modeling:

Task: Using a dataset provided by the Ministry of Health containing anonymized patient information such as age, gender, blood pressure, cholesterol levels, and other relevant attributes, your mission is twofold:

- Data Exploration and Analysis

- Predictive Modeling for Heart Disease Occurrence


The checklist for your Machine Learning Project:
## 1. Data Exploration (15 Points)
- To earn full points, you should interpret the results of your code.

### A. Data Profiling: Examining the overall structure and properties of the dataset, such as the number of rows and columns, data types, missing values, and basic statistics like mean, median, and standard deviation. 

### B. Data Visualization: Use histograms, scatter plots, ecdf, kde, box plots to explore the relationships, patterns, and distributions within the dataset. Analyzing these graphs, along with appropriate examples, will offer valuable insights and enable you to achieve maximum points.   

### C. Feature Exploration: univariate, bivariate, and multivariate analysis.

### D. Use the Groupby function to generate a minimum of two informative reports.

## 2. Dataset Preprocessing (15 Points)
### A. Handling Missing Data. Remove the unnecessary column(s) and explain why you think they are unnecessary. Use this clean dataset for the next tasks.

### B. Convert categorical values to integer: Convert categorical values to integers by detecting the categorical features and replacing them with your customized mapping. Report the distribution of the values in the categorical features if you did not do it in "1.Data Exploration".

### C. It seems data is sorted by "target". Shuffle the dataset and explain why the shuffling is necessary?

### D. Find the outliers in "chol" and "thalach" by computing maximum and minimum whisks. Report them then create a new dataset ("df_new") where outliers are not exist anymore. After this point use this new dataset. 

### E. Correlation Analysis: Present the correlation between features and "target" in both a list and a heatmap format. For the heatmap, include the six most strongly correlated features (positive and negative) with "target." Interprate the results.

### F. Examine the impact of age on 'trestbps', 'chol', and 'thalach' separately. Use regression plot and correlation matrix. Provide an interpretation of the results.

## 3. Model Development and Evaluation (40 Points)

### REGRESSION:

#### A. Use the clean dataset "df_new" from 2D and assign the 'thalach' to the variable "y" as output and the remaining features (including "target") to variable X. Next, normalize the features and assign normalized features to variable "X_norm". Explain the purpose of normalizing features. You may use any normalization technique.

#### B. Develop a multiple linear regression model (lm_1) by using all the features (X_norm) as independent variables and "thalach" as dependent variable. Report the R-squared (R²) score of the model and mean absolute error, then explain the results.
 
#### C. Perform Polynomial Regression with a degree of 2 on the dataset "X_norm". Afterward, compare the obtained results with the linear regression model lm_1 in B.

#### D. Create a pipeline that encompasses the Normalization (MinMax or Standard), Polynomial Transformation (degree of 2), and Linear Regression procedures. Test it by giving as input all the features (X) and check the R-squared score. Compare the result with the previous models.   

#### E. Determine the ideal polynomial order for X_norm by utilizing the R-squared (R²) scores of a linear model which is trained with the training dataset (X_norm_train, y_norm_train). Calculate the R-squared (R²) scores on the testing dataset (X_norm_test, y_norm_test). Compare the results to those obtained in "C" and provide an explanation if there are significant differences in the R-squared scores. (Hint: Degrees from 1 to 6 would be sufficient). 

#### F. Plot a graph that displays how R-squared (R²) scores on the testing dataset (X_norm_test, y_norm_test) vary with polynomial order. Then plot same graph for X_norm_train and y_norm_train. Analyze the graphs and explain the reasons for the differences between them.

### CLASSIFICATION:

#### A. Assign the 'target' to the variable "y_c" and the remaining features to variable "X_c" in "df_new" from 2D.
 
#### B. Utilize 4-fold cross-validation to X_c for assessing dataset homogeneity. Address any detected issues to ensure data integrity.

#### C. Normalize the feature values using min-max normalization.

#### D. To ensure the proper evaluation of the model's performance, it is necessary to divide the dataset (X, y) into training (X_train, y_train) and testing sets (X_test, y_test). For this purpose, we will allocate 20% of the dataset for testing.

#### E. Perform K-NN classification and find the score manually. Explain how you computed and interprate the score.

#### F. Select a classfier (except K-NN), explain how it works then perform classification for the dataset you got in 'D.' Then compare your model with the K-NN in "E." 

#### G. Find the value of k that maximizes the score of K-NN. Plot the k vs score graph. What is the percentage of false positive and false negative with the best performing solution? Give the confusion matrix and explain the results. 

#### H. Find the F1-score, precision, and recall on test data set and explain the results?
## 5. Presentation (30 points)
- You have two presentation options: Video or In-Person. Choose the one that suits you best.

    VIDEO Presentation: Create a video presentation, showcasing your code and report (in English). The video should not exceed 10 minutes. Please begin your video with a warm welcome and ensure your face is visible. This will help me to put your voice, a name and a face. You can record and upload your video via this link:   https://flip.com/37626232

    In-Person: The date/time and venue will be announced after project submission.  


- You can use this file or PowerPoint slides for your presentation.

- Team members should divide the workload equally: one member can deal with "1. Data Exploration" and "3. Model Development: Regression", while the other can handle "2. Dataset Preprocessing" and "3. Model Development: Classification". However, each team member is responsible for the whole project, not just the tasks assigned to them. Both should be capable of answering questions on all aspects of the project.

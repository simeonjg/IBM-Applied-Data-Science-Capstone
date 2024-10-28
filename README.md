# IBM-Applied-Data-Science-Capstone
This research attempts to identify the features that contribute to a successful rocket landing.

# Project Background
SpaceX is a leading innovator in the space travel industry that is able to perform many launches relatively inexpensively due to the reusability of their rocket, the Falcon 9. Our aim is to predict if the first stage of a launch of the Falcon 9 will land successfully, which is crucial to determining the cost of a launch.​

# Topics of Exploration
* How do payload mass, launch site, number of flights, and orbit affect the success of first-stage landing?​

* How does the rate of successful landings change over time?​

* What is the best predictive algorithm that can be used for the binary classification of a successful landing?​
  
# Methodology
1. Data Collection: SpaceX has data on launches and their outcomes available through their REST API. Using web scraping, we pulled this data and filtered it down to data for the Falcon 9 rocket. ​

2. Data Wrangling: The feature we are trying to predict is successful launches, but the data had multiple labels for launch outcomes. In order to conduct a binary classification, we converted this feature to binary labels of 0 or 1, indicating whether a landing was successful or not. ​

3. EDA: First, we used SQL commands to get summaries of the features in the data. Then we also leveraged Python libraries to get informative visualizations and conduct feature engineering on the data. ​

4. Interactive Visualization: We started by using Folium to interactively mark launch sites and launch outcomes on a map, also marking important locations around the sites. Then, we created an interactive dashboard using Plotly to show the launch outcomes for a chosen site or all sites in relation to payload mass. ​

5. Predictive Analytics: We split the data into train and test sets and fit multiple models to the training portion: Logistic Regression, SVM, Decision Tree, and K-Nearest Neighbors. We then evaluated these models on the test set to see which performed best for the binary classification.​

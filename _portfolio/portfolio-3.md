---
title: "Analysis of Flight Systems "
excerpt: "This project explores the enhancement of flight fare and delay predictions by merging conventional datasets with Twitter data, employing data processing and sentiment analysis to assess social media's influence on aviation trends."
collection: portfolio
---

### Do Twitter Insights Enhance Flight Fare and Delay Predictions?

In this project, I merged traditional flight data with sentiment-analyzed Twitter posts to enhance the accuracy of flight fare and delay predictions. This involved a series of steps including meticulous data cleaning, in-depth feature engineering, the application of machine learning models such as Random Forest, and comprehensive sentiment analysis. The objective was to capture the dynamic influence of social media on aviation industry trends.

## Flight Fare Prediction
* Performed Data Cleaning and feature engineering to get meaningful data features.
* Performed visualizations to understand how the target variable varies with various features such as Flight Duration and Number of Stops, amongst other comparisons. Generated plots for such comparisons.
* Performed One Hot Encoding and Test-Train Split on the data.
* Tested Various Machine Learning Regressions such as Linear Regression, Decision trees, Bagging Technique, and Random Forest and produced their Performance Metrics to achieve the highest-performing models.
* Random Forest turned out to be the best-performing model.

![image](/images/flight-scores.png)

The main aim was to successfully learn and find a way to superimpose relevant web-scraped data on the flight-fare dataset to introduce dynamicity (fluid market conditions) which could give us an idea about market conditions and ongoing socio-economic affairs that could affect flight fares.

## Twitter data mining
Scraped Twitter data using Twitter API and Tweepy library. Used keywords to extract over 10000 tweets and cleaned and processed them to perform sentiment analysis using the TextBlob library, calculate volumes, etc to structure it and extract useful insights.

## Augment Twitter data efficiently to improve predictions
* The question was if I could augment Twitter data efficiently to improve predictions on parameters such as flight delay and flight fares.
* Developed a random forest regressor with Twitter-less data and experimented with four kinds of data distribution styles - a combination of polynomial features, normalized target variable, and regular data to improve the model's performance. Using polynomial features and a normalized target variable reduced the mean squared error.
* Used the same procedure for Twitter augmented data as well, where our primary idea revolves around using more than the three additional features of polarity, subjectivity, and tweet volume for analysis.
* Could see very minor improvements in results but it strengthened the initial idea of using Twitter features to make predictions.

## Challenges faced
* The dataset was limited to information for February and March of the year 2022. Although it is a huge dataset with over 300,000 data points, it fails to give us enough information about the months before and after February and March 2022. One would need a dataset with more variation in months to successfully study the change in flight prices, infer valuable results, and observe interesting trends.
* Observed certain relationships between the ‘Date’ feature and the ‘Price’ target variable of our dataset which samples data from the year 2022 for February and March. We observe that there is a downward trend which indicates that on unique dates starting February through March, all airlines saw a drop in prices of flight fares. Soon after there was a surge in the prices due to the increase in jet fuel prices globally as observed in the graph on the right. The trending tweets around this decline period were COVID-related and rising tensions between Russia and Ukraine.
* However, it was not possible to derive interesting conclusions from such a smaller variation dataset and understand what role social media platforms such as Twitter play in this.

## Flight Delay Prediction
* Considered flight delay data related to weather conditions and scraped Twitter data for a common time (date-wise).
* Conducted sentiment analysis and produced three additional features that were used in the model - polarity, subjectivity, and tweet volume.
* Model 1 predicts delays based on weather information solely and Model 2 predicts delays based on weather information as well as augmented Twitter features.
* Loss values are compared to infer which is the better performing model, and consequently to understand whether Twitter features would be a useful addition for prediction.
* This showed how social media data provides insights.


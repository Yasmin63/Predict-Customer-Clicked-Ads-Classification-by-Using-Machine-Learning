![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/f8147632-7efb-475f-81d0-2378dd507f65)# Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning

## Background
"A company in Indonesia wants to know the effectiveness of an advertisement that they air, this is important for companies to be able to know how much the advertisement is marketed so that it can attract customers to see advertisements.By processing historical advertisement data and finding insights and patterns that occur, it can help companies determine target marketing, the focus of this case is to create a machine learning classification model that functions to determine the right target customers "



## Univariate Analysis
![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/48023c83-53e1-4012-aad3-aa0780c6fea2)

Interpretation:
The distributions of “Daily Time Spent on Site” and “Daily Internet Usage” features have a bimodal distribution.
The distribution of “Age” feature has a negatively skewed distribution
The distribution of “Area Income” feature has a positively skewed distribution



## Bivariate Analysis
![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/00ec7959-0543-44f8-9933-196f90cfe2de)

Interpretation:
Daily Time Spent on Site
- Customers with Daily Time Spent on Site 35 - 45 are more clicked on ad
- Customers with Daily Time Spent on Site 70 - 80 are more didn't clicked on ad
Age
- Customers with Age 35 - 45 are more clicked on ad
- Customers with Age 25 - 35 are more didn't clicked on ad
Daily Internet Usage
- Customers with Daily Internet Usage of 100 - 150 are more clicked on ad
- Customers with Daily Internet Usage of 175 - 225 are more didn't clicked on ad
Area Income
- Customers with an income range of around 380 - 460 million didn't clicked on ad more than those with other income ranges 



## Multivariate Analysis
![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/88288521-cd05-4ca4-b876-8852775e4b17)
Interpretation:
The “Daily Internet Usage” feature has a positive correlation with “Daily Time Spent on Site” feature equal to 0.52 and 0.34 with “Area Income” feature.
The “Daily Internet Usage” and “Age” features have a negative correlation equal to -0.37
The “Daily Time Spent on Site” feature has a negative correlation with “Age” feature equal to -0.33



## Data Cleaning and Preprocessing
- Handling missing value. There are 4 features that have null values: “Daily Time Spent on Site”, “Area Income”, “Daily Internet Usage” and “Gender”. The four features are filled with median and mode values.
- Handling outlier using z-score method.
- Feature extraction. Create a new table of year, month, week and day from the timestamp column.
- Feature encoding. Clicked on ad and gender column.
- Feature selection. Drop unused columns: timestamp, category, city, province
- Split Data based on clicked on ad column.



## Data Modeling
Modelling Without Normalization & Standarization

![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/6cb90d9a-3f23-4d02-817f-273fe2520df7)

Modelling With Normalization & Standarization

![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/93221356-3abf-4910-ab8f-ff655c1d8d53)

![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/48f08239-e67a-4341-84a2-58e317143a9c)

Top four features to predict advertisements clicked by customers are Daily Internet Usage, Daily Time Spent on Site, Area Income, and Age. Daily Internet Usage has the highest importance score highest, followed by Daily Time Spent on Site. This shows that the higher the daily internet usage and daily time spent on site, the higher the likelihood of customers to click on ads.In addition, customers with higher area incomesand younger age are more likely to click on ads as well. 



## Business Recommendation & Simulation

![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/4890bc03-4b1a-4a13-a033-2d66e283140c)

Top four features to predict advertisements clicked by customers are Daily Internet Usage, Daily Time Spent on Site, Area Income, and Age. Daily Internet Usage has the highest importance score highest, followed by Daily Time Spent on Site. This shows that the higher the daily internet usage and daily time spent on site, the higher the likelihood of customers to click on ads.In addition, customers with higher area incomesand younger age are more likely to click on ads as well. 

![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/158728ef-d176-4ea8-94f5-e2dff03a5baf)

- Customers with daily internet usage of 100-140 and 141-180 had the highest percentage who clicked on the ads. This shows that they do not have the time and are more likely to be interested in the advertised service. Companies can give special promos so that customers will not only click on the ad but will buy products.
- Improve and optimize advertising promotions to target customers who have a high percentage of not clicking ads with daily internet usage between 181-225+. The company needs to further analyze such as adjusting ad content and targeting to better match interests.

![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/b14afbfd-b5d6-4c68-8a0c-3c1d4c07983a)

- Customers with daily time spent on the site 30-70 have the highest percentage of customers who clicked on the ads. This indicates that they are interested in the product orservice being advertised. Adjust your ad targeting strategy and improve user experience. This may include improving website design and usability of the website, providing clear and concise ad content, and ensuring that ad placements are visible and attractive to potential customers to potential customers.
- Customers with time spent on the site each day >70 have the highest percentage of not clicking on ads. it is important to optimize the advertising campaign by adjusting the advertising content and targeting to better suit their interests and preferences. This can be achieved by analyzing their behavior on the website, conducting surveys to understand their needs or interests, and providing appropriate promotional offers or products to encourage them to click through.or appropriate products to encourage them to click and buy.

![image](https://github.com/Yasmin63/Predict-Customer-Clicked-Ads-Classification-by-Using-Machine-Learning/assets/146631940/301d2459-d7d6-4f58-a2cd-8533f7614e78)

- In overall out of 300 sample customers, machine learning will predict 143 customers not click the ad and 157 customers click the ad or 48% and 52%.
- Based on confusion matrix table beside machine learning created successfully correctly predict customers who did not clicked on the ad by 137 customers out of a total 300 sample customers or 46%.
- From 157 customers who were predicted to click ads by machine Learning 153 customers were predicted correctly or 97%. While the rest about 3% are errors









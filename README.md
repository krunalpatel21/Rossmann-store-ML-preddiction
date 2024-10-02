Project Name - Retail Sales Prediction
Project Type - Regression
Contribution - Krunal Patel
Project Summary -
Rossmann, a retail chain, operates an extensive network of over 3,000 pharmacies across seven European countries. Presently, the store managers at Rossmann face the challenge of forecasting their daily sales for the upcoming six weeks. Numerous factors such as promotions, competition, school and state holidays, seasonal variations, and local demographics affect the sales performance of each store. Given the diverse circumstances of individual managers, the accuracy of sales predictions tends to vary significantly.
Problem Statement
We have access to historical sales data from 1,115 Rossmann stores. Our objective is to predict the "Sales" column for the test set. It's worth noting that some stores in the dataset were temporarily closed due to renovation work.
Data Description
The dataset includes two main files:

Rossmann Stores Data.csv: This file contains historical data, including sales information.

store.csv: This file provides supplemental details about the stores. Data Fields:

Id: An identifier representing a combination of store and date within the test set. Store: A unique identifier for each store.

Sales: The turnover for a particular day (this is the target variable for prediction).

Customers: The number of customers on a given day.

Open: An indicator of whether the store was open (0 = closed, 1 = open).

StateHoliday: Indicates a state holiday; typically, stores are closed on these days. Types include a = public holiday, b = Easter holiday, c = Christmas, 0 = None.

SchoolHoliday: Indicates if the store was affected by the closure of public schools on that date.

StoreType: Differentiates between four store models: a, b, c, d.

Assortment: Describes the assortment level: a = basic, b = extra, c = extended.

CompetitionDistance: The distance in meters to the nearest competitor store.

CompetitionOpenSince[Month/Year]: Approximate year and month when the nearest competitor store opened.

Promo: Indicates whether a store is running a promotion on that day.

Promo2: Indicates whether the store is participating in a continuing and consecutive promotion (0 = not participating, 1 = participating).

Promo2Since[Year/Week]: Describes the year and calendar week when the store started participating in Promo2.

Conclusion

PromoInterval: Describes the consecutive intervals when Promo2 is initiated, listing the months the promotion begins anew. For example, "Feb,May,Aug,Nov" indicates that the promotion restarts in February, May, August, and November of any given year for that store.
In light of the evaluation results, it's evident that all three machine learning models, Linear Regression, Lasso Regression, and Decision Tree, exhibit varying levels of performance in predicting the target outcome.

Both Linear Regression and Lasso Regression models demonstrate similar predictive capabilities, with R-squared scores around 0.78 and Mean Squared Error values close to 0.78 as well. This suggests that they offer reasonable predictive accuracy and can effectively capture the relationships between the independent and dependent variables in the dataset.

On the other hand, the Decision Tree model stands out with remarkable performance, achieving an exceptionally high R-squared score of nearly 1 (0.999996) and a relatively low Mean Squared Error of 0.9158. These results indicate that the Decision Tree model almost perfectly predicts the target outcome and exhibits minimal prediction errors.

However, it's crucial to consider the potential drawbacks of the Decision Tree model, such as its susceptibility to overfitting, particularly in complex datasets. Despite its outstanding performance in this evaluation, further scrutiny is necessary to ascertain its generalization ability and suitability for real-world applications.

In conclusion, while all three models showcase distinct strengths and weaknesses, the Decision Tree model emerges as the top performer in terms of predictive accuracy for the given dataset. Nonetheless, careful consideration of the specific requirements and characteristics of the application domain is essential in selecting the most appropriate model for deployment.

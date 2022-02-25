# Thinkful-Capstone-2
Supply Chain: Predicting the Final Delivery Status of Shipments and the Actual Number of Days Spent in Transit
Source: https://www.kaggle.com/saicharankomati/dataco-supply-chain-dataset

For this supervised machine learning project, I would like to see whether Decision Trees or Random Forests are better for predicting the delivery status of a shipment using features such as payment type, shipping mode, number of days expected in transit, and whether the shipment is international or not. I would also like to see whether OLS or KNN is the better regression model for predicting the actual number of days the shipment spends in transit using the mean squared error (MSE) as the metric.

I used various Python packages to run the tests and discovered that for classification, the Decision Trees and Random Forests had similar accuracy, precision, recall, and F1 scores. It was surprising that domestic shipments were more often late than international ones. Similarly, somehow shipments with scheduled shipping of greater than 3 days or less than a day were on time while those in between are all predicted to be late. It was not surprising that shipments with faster payment methods were likely to be on time. Another relevation was that only the shipments with the fastest shipping method were predicted to be on time. As a whole, given that the Decision Tree is simpler, it is the better model for classifying on-time or late.

For the regression in predicting the number of days in transit, each upgrade in the shipping mode resulted in an average 3.5 day decrease in the actual number of days spent in transit. I also discovered that for every one day increase in the expected number of shipping days, the actual number of days spent in transit decreased by almost 2 days. Neither the payment type nor the international status of the shipment were significant enough in the final OLS model. Overall, the OLS model had the lower MSE, making it better than the KNN one.

This is intended for shipping companies to update shipping/delivery statuses and estimate the number of days spent in transit.

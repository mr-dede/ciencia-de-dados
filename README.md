# final project

This project was done as the final work of the course: "Data Scientist Training: The Complete Course [2023]" available on the Udemy platform. The objective was to restore the database of a financial company, whose default rate was 30%, and, through Machine Learning techniques, reduce it to at least 25%.

After appropriate data processing, I developed six predictive models. Although these models have similar hit rates, they identify defaulters with high accuracy. However, some are overly conservative, which means they tend to improperly classify good customers as defaulters.

Assessment Method:

1. Defaulters Incorrectly Classified as Good Payers: By multiplying the number of defaulters by the average value of the loans, I estimated the potential loss.

2. Incorrectly Classified Good Payers: For those who were wrongly denied, I calculated the lost revenue based on the compound interest the company failed to receive.

3. Potential Profit: For correctly identified good payers, I determined the profit based on the total interest received minus the total loss.

Results:

- Model 1: Loss: 107222.66, Profit: -100074.48, Default: 0%
- Model 2: Loss: 62246.93, Profit: 30679.37, Default: 5.5%
- Model 3: Loss: 92926.30, Profit: -71481.77, Default: 0%
- Model 4: Loss: 81682.37, Profit: -38793.31, Default: 1%
- Model 5: Loss: 48452.85, Profit: 65917.98, Default: 6.5%
- Model 6: Loss: 55639.81, Profit: 15841.95, Default: 1.7%

Note that the default rate for each model was calculated considering the proportion of "good-bad" (defaulters classified as good payers) in relation to the 290 customers in the test set.

Given the stated objective of reducing the default rate to at least 25% and the results above, Model 5 appears to be the most promising. Not only does it have the lowest loss, but it also offers the highest profit and has an acceptable default rate of 6.5%.

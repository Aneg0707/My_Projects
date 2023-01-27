# Website-Parsing-Regression-for-Price-Prediction
Website Parsing + Regression for Price Prediction 
for Artificial Intelligence in Marketing class, St. Lawrence college
Business analytics

The project instructions:
- Create a dataset by parsing the webpage used in class.  This is the base URL (https://admn5015-340805.uc.r.appspot.com/2019-01-01.html).  
- Download these fields (date, price, likes, dislikes, and followers) for each day by changing the URL accordingly, starting on January 1st, 2019 until December 31st, 2022.
- Clean the data if needed.
- Save your downloaded dataset as a CSV file.
- Use the regression models and predict the price of the website's product (you would be predicting the price for January 1st, 2023).
- Make sure you choose the algorithm with the lowest RMSE for your prediction.
- Your assignment must include the different visualizations available in the original Regression template.
- You should upload your Python project, and a PDF file summarizing your assignment (you can include screenshots or your exported iPython Notebook).

Steps being made during the project:
1)	Table with dates was created to link them with the webpages
2)	Table with dates was transformed into a table of webpages
3)	Each link was parsed, and data was saved in a data frame
4)	Data cleaning
5)	Data frame with parsed data was saved in a CSV
6)	Data column was transformed to the Gregorian ordinal of the date, so we can use that in regression (1 Jan of Year 1 = 1, 2 Jan of Year 1 = 2 and so on).
7)	Split for train data (75%) and test data (25%)
8)	Random Forest Regressor was the best model based on the RMSE = 22
9)	Prediction is made for 1 Jan 2023, 10,000 likes, 500 dislikes, 17,000 followers – price is 11476.32 (Gregorian ordinal of the date is 738521, as the previous day is 738520)





NOTE: the independent variables show high level of correlation – Multicollinearity may take place, which may create overfitting problem in the model.

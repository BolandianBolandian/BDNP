# BDNP
a Machine Learning model for predicting the future of the USD/IRR and stock market in Iran.

### What made me think of making this ML model?
According to the several years of experience I had in trading the Iranian stock market and USD/IRR,some patterns were formed at different points in the stock market and USD/IRR market at the same time, which recently attracted my attention.
You can see some of these patterns in the figure below.<br><br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="https://private-user-images.githubusercontent.com/104448040/320200771-388b8d13-4107-45d0-ac44-ceb18732077d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI0MDI4NTcsIm5iZiI6MTcxMjQwMjU1NywicGF0aCI6Ii8xMDQ0NDgwNDAvMzIwMjAwNzcxLTM4OGI4ZDEzLTQxMDctNDVkMC1hYzQ0LWNlYjE4NzMyMDc3ZC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQwNlQxMTIyMzdaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT04MzcxNGMwNDZiYjMzMjc0OWI0MWUxODQwYTgzZDIxNDc1Y2UwMGRmZDc5MjBmOGZmOWMxZGYxYzQ4YWY1MWZlJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.n88jI2VdUKYjJ7uYQjfRDoF0T5_-PtJLwaiI79ny418" alt="USD/IRR and Iranian Stock Index chart" width="800" height="600"><br><br><br>
As it is obvious, the correlation between the Iranian stock market and USD/IRR rate is not always constant and is sometimes negative and sometimes positive. Sometimes, both the trend of USD/IRR and the trend of the Iranian stock market index are rising at the same time, but their growth rates are completely different (pattern A). Sometimes the trend of USD/IRR is upward, but the trend of the Iranian stock market index is downward (pattern B), and sometimes the trend of USD/IRR is downward, but the trend of the Iranian stock market index is upward (pattern C). Such patterns can be found in abundance in the chart of them.
The point that forced me to create an ML model to discover the secret of the formation of these different patterns in different time frames was that these patterns are never formed by chance and I am sure there is a logic and algorithm behind it that i think only machine learning methods can discover.

### How does this ML model work?
In general, the mission of this ML model is to predict the best market for investment in the next period, this is why we call it "BDNP" -Best Decision for Next Period- . in this way, different information (30 features) from the Iranian stock and the USD/IRR market is given to the model and it makes the desired prediction for us.
In other words, this model was created to answer this question:
In the next 6 days in IRAN, if I have some money to invest, which is the best option between the Iranian stock market and the US dollar?<br>
You can see part of the data given to the model [here]()


### Why the next 6 days?
You probably know that Iran's economy is unstable with high annual and monthly inflation. for Example you can see the USD/IRR rate in last 14 years below:<br><br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="https://private-user-images.githubusercontent.com/104448040/320202324-9c70ab09-ff10-4fbf-8259-bdddc9ef44fa.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MTI0MDQ3MDYsIm5iZiI6MTcxMjQwNDQwNiwicGF0aCI6Ii8xMDQ0NDgwNDAvMzIwMjAyMzI0LTljNzBhYjA5LWZmMTAtNGZiZi04MjU5LWJkZGRjOWVmNDRmYS5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwNDA2JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDQwNlQxMTUzMjZaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT00MWU0M2E5MzFlMzhhODAxODViOWQzYWM1ZGU3ZWMwNDg1ZjAyZWI3YzNjZjJlMjY5Yzc0ZGY2MzNkOTk1YWEyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.dCQb7cPjyh-94mpQzd2IlDO2gj2MjgcI-MvlFfy3flo" alt="USD/IRR rate in last 14 years" width="800" height="600"> <br><br><br>
According to these rapid fluctuations of economic parameters and the information we had from the archives of the Iranian stock and USD/IRR market, and many investigations that took place, we concluded that the created ML model will have the highest efficiency and the most accurate forecast for 6-day periods (working days), so the inputs of The model is in the form of 6-day periods and the output of the model is also suitable for 6-day periods.

### How accurate is this model working?
In the tests, the mentioned model was able to make its predictions with 70% accuracy, in other words, out of every 10 predictions it made, it had only 3 errors, and this percentage of accuracy is very important in the financial markets and According to financial market experts, it is considered amazing.
Keep in mind that the output of this model, in the determined time intervals, can be placed next to the strong technical analysis performed by the specialist in that field and increase its accuracy with this work and increase the validity of its prediction.

### How to trust in this ML model? Let`s check it out.
Since it is not possible for me to publish the complete code written to build the BDNP model, I intend to publish the outputs of the model [here](https://github.com/BolandianBolandian/BDNP/tree/main/Model%20Predictions), period by period, and after the completion of each period, I will post a report based on the evaluation of the prediction in the relevant section. 


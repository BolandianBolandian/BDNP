# BDNP
an amazing Machine Learning model for predicting the future of the USD/IRR and Iranian stock market.

### What made me think of making this ML model?
According to the several years of experience I had in trading the Iranian stock market and USD/IRR,some patterns were formed at different points in the stock market and USD/IRR market at the same time, which recently attracted my attention.
You can see some of these patterns in the figure below.<br><br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="https://github.com/BolandianBolandian/BDNP/blob/main/images/USD-IRR%20and%20Iranian%20Stock%20Index%20chart.png?raw=true" alt="USD/IRR and Iranian Stock Index chart" width="800" height="600"><br><br><br>

As it is obvious, the correlation between the Iranian stock market and USD/IRR rate is not always constant and is sometimes negative and sometimes positive. Sometimes, both the trend of USD/IRR and the trend of the Iranian stock market index are rising at the same time, but their growth rates are completely different (pattern A). Sometimes the trend of USD/IRR is upward, but the trend of the Iranian stock market index is downward (pattern B), and sometimes the trend of USD/IRR is downward, but the trend of the Iranian stock market index is upward (pattern C). Such patterns can be found in abundance in the chart of them.
The point that forced me to create an ML model to discover the secret of the formation of these different patterns in different time frames was that these patterns are never formed by chance and I am sure there is a logic and algorithm behind it that i think only machine learning methods can discover.

### How does this ML model work?
In general, the mission of this ML model is to predict the best market for investment in the next period, this is why we call it "BDNP" -Best Decision for Next Period- . in this way, different information (32 features) from the Iranian stock and the USD/IRR market is given to the model and it makes the desired prediction for us.
In other words, this model was created to answer this question:
In the next 6 days in IRAN, if I have some money to invest, which one is the best option between Iranian stock market, US dollar and Fixed-income investment funds?<br>
You can see part of the data given to the model [here](https://github.com/BolandianBolandian/BDNP/tree/main/Data)


### Why the next 6 days?
You probably know that Iran's economy is unstable with high annual and monthly inflation. for Example you can see the USD/IRR rate in last 14 years below:<br><br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <img src="https://github.com/BolandianBolandian/BDNP/blob/main/images/USD-IRR%20rate%20in%20last%2014%20years.png?raw=true" alt="USD/IRR rate in last 14 years" width="800" height="600"> <br><br><br>
According to these rapid fluctuations of economic parameters and the information we had from the archives of the Iranian stock and USD/IRR market, and many investigations that took place, we concluded that the created ML model will have the highest efficiency and the most accurate forecast for 6-day periods (working days), so the inputs of The model is in the form of 6-day periods and the output of the model is also suitable for 6-day periods.

### How accurate is this model working?
In the tests, the mentioned model was able to make its predictions with 70% accuracy, in other words, out of every 10 predictions it made, it had only 3 errors, and this percentage of accuracy is very important in the financial markets and According to financial market experts, it is considered amazing.
Keep in mind that the output of this model, in the determined time intervals, can be placed next to the strong technical analysis performed by the specialist in that field and increase its accuracy with this work and increase the validity of its prediction.

### How to trust in this ML model? Let`s check it out.
Since it is not possible for me to publish the complete code written to build the BDNP model, I intend to publish the outputs of the model [here](https://github.com/BolandianBolandian/BDNP/tree/main/Model%20Predictions), period by period, and after the completion of each period, I will post a report based on the evaluation of the prediction in the relevant section. 
##### Attention:
To compare the amount of changes in the USD/IRR market compared to the Iranian stock market, if the total index of the Iranian stock market is used to compare with USD/IRR, we will not get the correct result because, for several reasons, the total index of the Iranian stock market does not represent the state of the entire stocks in the market and deliberate manipulations by the market maker is evident in this index in different time frames.
Therefore, in order to more closely examine the overall changes in the Iranian stock market, we have used the average changes of 4 stock investment funds named Dariush, Kardan, Agas and Asas.


# What does this file contain?
Obviously, it is not possible to mention all the features used in model training clearly and precisely, but in general, it should be said that features 
such as USD/IRR rate, stock market index, stock market transaction value, stock market value in USD, etc. is used in this section.
In this sample file, in general, the names of the features are named from F1 to F30, and the last column is the prediction column and it is formed with
three different states 0, 1 and 2. <br>
0 means 'IRR', 1 means 'USD' and 2 means 'Iranian Stock'.
each prediction is made for next period, according to its row data. 
for example in the first row, prediction is equal to 1, that means If you change your assets
into US dollars now, you will get the highest return in the next period (next 6 business days) compared to the Iranian stock market and the Iranian Rial.
for another example in the last row, prediction is equal to 0, that means If you change your assets
into Iranian Rial now, you will get the highest return in the next period (next 6 business days) compared to the Iranian stock market and the US dollar.


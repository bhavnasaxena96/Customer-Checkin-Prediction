# Customer-Checkin-Prediction

Bonus Problem Solution

Write about any difficult problem that you solved. (According to us difficult - is something which 90% of people would have only 10% probability in getting a similarly good solution).

This might not seen as a problem but almost every one has faced situations where we have to take decision at the moment where we have to decide whom to choose among us or other, such a similar problem was with me, where I and my friend who was in different school ,she was getting late for her exam and mine was also on the same day ,so the situation was I have to decide whether to drop her or just leave alone for my exam ,
but at that moment I decided to  drop my friend and successfully reached at my location to and we both gave our exam .

Explain back propagation and tell us how you handle a dataset if 4 out of 30 parameters have null values more than 40 percentage

(a)deleting rows:
This method commonly used to handle the null values. Here, we either delete a particular row if it has a null value for a particular feature and a particular column if it has more than 70-75% of missing values. This method is advised only when there are enough samples in the data set. One has to make sure that after we have deleted the data, there is no addition of bias. Removing the data will lead to loss of information which will not give the expected results while predicting the output.
(b) Replacing With Mean/Median/Mode
This strategy can be applied on a feature which has numeric data like the age of a person or the ticket fare. We can calculate the mean, median or mode of the feature and replace it with the missing values.
(c) Using Algorithms Which Support Missing Values
KNN is a machine learning algorithm which works on the principle of distance measure. This algorithm can be used when there are nulls present in the dataset.

Part 1 problem solution
QUES :
Write a regex to extract all the numbers with orange color background from the below text in italics.
{"orders":[{"id":1},{"id":2},{"id":3},{"id":4},{"id":5},{"id":6},{"id":7},{"id":8},{"id":9},{"id":10},{"id":11},{"id":648},{"id":649},{"id":650},{"id":651},{"id":652},{"id":653}],"errors":[{"code":3,"message":"[PHP Warning #2] count(): Parameter must be an array or an object that implements Countable (153)"}]}
SOLUTION:
import re
text = '{"orders":[{"id":1},{"id":2},{"id":3},{"id":4},{"id":5},{"id":6},{"id":7},{"id":8},{"id":9},{"id":10},{"id":11},{"id":648},{"id":649},{"id":650},{"id":651},{"id":652},{"id":653}],"errors":[{"code":3,"message":"[PHP Warning #2] count(): Parameter must be an array or an object that implements Countable (153)"}]}'
l = [i for i in re.findall(":(\d*)",text) if i]
print(l)
OUTPUT:
['1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '648', '649', '650', '651', '652', '653', '3']
Note: solution also shown in screencast video.


# Predicting World-Happiness

Can happiness be predicted? Most would say that is a very subjective question, but the Gallup World Poll and the UN may have a tool that can answer that question using data. The World Happiness Report has been a survey conducted of 155 countries for the last several years that measures happiness based on different factors. <br>
For this project, I have taken data from the report over the last several years to see if a prediction model can be built to predict a happiness score. Initial analysis showed strong correlations between certain values that were used in the measurement and the overall score, while other values had very little correlation to the final score. <br>
I began using a linear regression model and the r-squared score came out to 76% for the testing set. Next, I used Random Forest and the first run was with only 10 decision trees and gave a score of 79% for the testing data set. This was better than the linear regression, so I ran it again, with a bigger forest of 10,000 trees and got a test score of 82%. I had also used a much larger forest, using 100,000 trees, but the score for the testing data was essentially the same so I kept the 10,000 trees. <br>
Since Random Forest performed the strongest, I used that algorithm for my predictions. My final predictions were very close to the actual happiness scores, with most coming within 0.4 points of the actual score. There is still room for improvement, but the predictions are promising. <br>
During the initial analysis, I took a look at the factors that were more correlated to the overall happiness score, like GDP and Health, and this information could be useful for further investigation into the model. Looking forward I would be interested to see how those would be on their own at predicting the happiness score.

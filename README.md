# WholeFoods
Exploring Whole Foods Locations by Demographics


To examine the demographics of counties where there were Whole Foods, I built a classifier that took in county demographic data and predicted whether or not that county had a Whole Foods. Building a predictive model had a few benefits:
  - Going through over 100 demographic statistics by hand is unweildy even with computer assistance. A Predictive model yields information on which features are most relevant to it's predictions and helps focus attention on most salient demographics
  - Looking at counties that my model got wrong could be areas worth exploring as possible locations for new Whole Foods Stores
 
Additonally I scraped all locations nationwide for related and competing buisnesses with the hopes that this data would be predictive of WholeFoods Locations. Companies included Starbucks, McDonalds, Target, Walmart, and Trader Joes.
 
I used 2 classifiers to generate predictions and narrow down features. Logistic Regression with L1 (Lasso) regularization and Gradient Boosted Trees. For feature selection, I used a combination of features that had non-zero coefficients for the Lasso and features that were above a given threshold for the Gradient Boosted Trees features importances. This narrowed down my feature set to a size of 30 while still maintaining a nice diversity of demographic statistics. Interestingly, ethnicity statistics were mostly filtered out and seemed to play an insignificant role in my models predictive accuracy.

The single most important variable turned out to be starbucks locations. Trader Joes locations were also in the top 3 so my theory on related buisnesses turned out to be quite useful. 

Other important features were pretty much as expected: Wholefoods tend to be located in urban areas, with a high proportion of college graduates and families earning greater than $75K.

Another interesting thing to note was the negative correlation with obesity rates. 92% of all Whole Foods stores were in counties where obesity rate was less than the median (31%). 

You can see the slides I used to present this project [here](McNultyFinal.pptx), the python code for [analysis](Analysis.ipynb) and a d3 visualization of demographics across the country [here] (http://bl.ocks.org/rshap91/raw/7d83217a05828988c6f543acfa2f887c/)

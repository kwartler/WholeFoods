# WholeFoods
Exploring Whole Foods Locations by Demographics

Need to write Intro...


To examine the demographics of counties where there were Whole Foods, I built a classifier that took in county demographic data and predicted whether or not that county had a Whole Foods. Building a predictive model had a few benefits:
  - Going through over 100 demographic statistics by hand is unweildy even with computer assistance. A Predictive model yields information on which features are most relevant to it's predictions and helps focus attention on most salient demographics
  - Looking at counties that my model got wrong could be areas worth exploring as possible locations for new Whole Foods Stores
 
 
I used to classifiers to generate predictions and narrow down features. Logistic Regression with L1 (Lasso) regularization and Gradient Boosted Trees. For feature selection, I used a combination of features that had non-zero coefficients for the Lasso and features that were above a given threshold for the Gradient Boosted Trees features importances. This narrowed down my feature set to a size of 30 while still maintaining a nice diversity of demographic statistics. Interestingly, ethnicity statistics were mostly filtered out and seemed to play an insignificant role in my models predictive accuracy.

The unanimous 
 




http://bl.ocks.org/rshap91/raw/7d83217a05828988c6f543acfa2f887c/

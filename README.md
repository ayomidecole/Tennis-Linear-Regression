# Tennis Linear Regression

The goal of this project was to find what features in the dataset best predict Winnings (we all love some $$$). To accomplish this, I used single feature linear regression and multiple feature linear regression.

## Steps
1. The first step was to investigate the data. The main approach here was to do a simple correlation analysis, the first step was a correlation between Wins and Winnings. This had a strong correlation of 0.91. I also looked at how other fratures were correlated with Wins, not super strong logic but if a feature correlates highly with Wins that feature probably is a good indicator of Winnings.
   
2. The next step was a single feature regression. Our target feature (dependent variable) which we are trying to describe is Winnings. I looked at which features would be good to use to predict Winnings. These are some of the model scores:
   * The model score of the feature Wins in this run is 0.8162457151181385
   * The model score of the feature Aces in this run is 0.6030848867880199
   * The model score of the feature Break Point Opportunities in this run is 0.8671468923973805
     
  From these model scores we can see the best feature to use to predict winnings based on this dataset in Break Point Opportunities.
  
3. The next step was multiple feature regression. In the code you can see the different feature sets I picked gave us similar model scores (around 0.85). It would assume that because Wins and Break Point opporutnities are strong features, they kinda hijack the model. At this point I do not know any sophisticated way to test this hypothesis but to work around that I trained a model after taking out those two features and indedd it did perform worse (score of 0.68)

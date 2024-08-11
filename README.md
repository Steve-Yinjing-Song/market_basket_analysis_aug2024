# Grocery Store Market Basket Analysis

## Problem Statement 

The retail sector is especially benefiting from machine learning. One such prominent retail 
use of machine learningis market basket analysis(MBA). Knowing which goods customers frequently 
buy together enables merchants to organize their stores and website consistently. It is mostly
accomplished by looking at their purchase behavior. Busineses use it as a cross-sell tool.

## Project Process

-- Data Collection
The datset we chose to use consists of 37,865 observations. There are three columns: Memmber_
numer, Date and Item_description. 

-- Data preprocessing
First of all, we removed the duplcates to keep every data point unique. we are trying to figure
out the possibility of co-occurence between products or product combinations. The purchaing 
volume doesn't matter.
We then created a new column Transaction_ID by concatenating the column MemberNumber and Date.

## Apriori Algorithm

The method for creating the baskets is called Apriori algorithm. We took  a threshold occurrence 
0.001. Any items that are less than this threshold are removed from further analysis. We then 
built association rules by setting metric as Lift  and min threshold as 1. By definition, the 
metric Lift measures how much we have lifted the purchase likelihood of the consequent by having
antecedent included in thr basket. A values of 1 represents no increase.

## Conclusion

By sorting the metric Lift descendingly, we can see what products or product combinations occur
together than expected if their purchase frequencies were independent. (sausage) and (whole milk,
yogurt) have highest Lift score. So we can promote them together in marketing campaigns to 
drive up more sales.  

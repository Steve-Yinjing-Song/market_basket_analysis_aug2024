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


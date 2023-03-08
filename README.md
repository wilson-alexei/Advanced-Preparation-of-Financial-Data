# Advanced-Preparation-of-Financial-Data

## Overview of the Project
Understanding pricing strategies in the context of the Initial Public Offering (IPO) process has been receiving much attention. Most prior studies have however focused on information sources from post issuance periods, and understanding such strategies from the management’s perspective during the IPO process is still an open research issue. Form 424 variants, as the finalized IPO prospectus approved by Security Exchange Committee (SEC), contain rich and genuine information about the issuing firms. In this study, we analyze the inter-relationships between the management’s confidence (through the proxy of sentiments expressed in textual contents in the Management’s Discussion & Analysis (MD&A) sections in the prospectus) and the pre-/post-IPO valuations.

In this competition, we are provided with data regarding successful U.S. IPOs from more than 600 companies. Our client is seeking advanced and novel methods to prepare the collected data, for further predictive analysis of the “underpricing” phenomenon. We will mainly focus on the data understanding and data preparation phases in the CRISP-DM model. 

## Project Guidelines

### Research Question
The overarching research question is “ How to predict the IPO underpricing phenomena? ” In this project, our main purpose is to prepare the data for predictive models answering the overarching research question. We also come up with additional RQs such as "what are the determinants of the PO underpricing phenomena?"

### Tasks
Following tasks are conducted in data preparation phase:

* Descriptive statistics – describing the data using minimum, maximum, 1st & 3rd quartile, mean, median, standard deviation, number of records, number of missing records, ...
* Imputation – dealing with missing data, you can choose from following strategies: i) drop the record with missing (highly discouraged); ii) replace the missing with mean/median/mode, determined on the data type; iii) replacing missing values in continuous field with linear regression predictions;
* Normalization – You need to manipulate all continuous fields to follow normal distribution: which contains two steps: i) removing skewness (using logarithm, square root, etc.) ii) make sure the residual is randomly distributed;
* Correlation analysis – you need to select predictor variables with low pair-wise correlation (i.e. Pearson's R) values – usually the threshold is 0.5 – one variable from the pair should be excluded from the model;
* Standardization – you need to convert the values at the same numeric level; one way of doing this is to use the z-score standardization, which is calculated as shown on this page.
* Recoding – for categorical data, you might want to recode them. For instance, since you need to use AUC as the evaluation metric, you should convert the target(s) to binary (two classes). Also, you should recode any categorical variable(s) with no more than 5 classes.

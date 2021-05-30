# Artificial-Intelligence-for-Finance: Predicting Defaultation on Credit Cards

## Purpose:
The purpose of this project was to analyze a data set of a given set of credit cards and to correctly predict if a person was going to default or not on their cards based on their previous history and the history of others.

![Credit Card](https://thumbs.dreamstime.com/b/here-generic-credit-card-isolated-al-white-background-logos-type-generic-here-generic-credit-card-isolated-125482245.jpg)
Please see the powerpoint for an overview of the case study [here](https://drive.google.com/file/d/1hBkihdzcTzu7ux6WfQoiqADsdA9tbz8j/view?usp=sharing), or see the comments in the jupyter file for more detail.

## Data Set:
The data set given was based on a [Kaggle Database](https://www.kaggle.com/mariosfish/default-of-credit-card-clients).

This data set had the following variables: history of payment, demographic factors, default payments, credit data, and bill statements. The information was based on people in Taiwan from April 2005 to September 2005.

The variable that was targeted was the default.payment.next.month, where 1 = default and 0 = not defaulted, which was based solely on if they defaulted or not in October of 2005. The 24 features included how much the client owed each month, what the client's payment status was, and the amount paid by the client for each month.

This given dataset simulated a real world situation as the dataset had inaccurate labels for default payment next month, the target variable, the payment status and was not precleaned. To further complicate the dataset, it was not clearly explained how to read the dataset clearly. What each variable means and how to properly implement them into our model, please check the juypter file.

## Methods:
The methodology used was to conduct an EDA, clean the dataset, and then the creation of multiple models to see which one would estimate the best.

## Results:
A Gaussian Naive Bayes model was used as it had the best on recall prediction with a value of 89%. Recall was chosen as the benchmark as it was more prudent to predict which customers are likely to have default payments next month or not. Rather than overestimate the potential loss/short of income flow than underestimate it in the perspective of cash flow control and risk management. Therefore, it was more important to identify as many default customers as possible even though some of them did not actually default.

### Based the EDA some key finds were found:

Three variables had the highest correlation if a person would default in October or not.
    * They had defaulted in August
    * If they were male
    * Their education level was high school level

## Conclusion:

The bank should be watchful of males who have defaulted two months prior to the current month and they have a high school education level, as they are more likely to default then others.


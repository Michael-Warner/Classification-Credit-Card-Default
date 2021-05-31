# Artificial-Intelligence-for-Finance: Predicting Defaulting on Credit Cards

## Purpose:
The purpose of this project was to analyze a dataset of a given set of credit cards and to correctly predict if a person was going to default or not on their cards based on their previous history and the history of others.

![Credit Card](https://thumbs.dreamstime.com/b/here-generic-credit-card-isolated-al-white-background-logos-type-generic-here-generic-credit-card-isolated-125482245.jpg)

Please see the powerpoint for an overview of the case study [here](https://drive.google.com/file/d/1hBkihdzcTzu7ux6WfQoiqADsdA9tbz8j/view?usp=sharing), or download our [jupyter file](https://github.com/Zexes9/Credit-Card-Default/blob/main/Default%20of%20credit%20card%20clients.ipynb) for more detailed comments.

## Data Set:
The dataset given was based on a [Kaggle Database](https://www.kaggle.com/mariosfish/default-of-credit-card-clients).

This dataset had the following variables: history of payment, demographic factors, default payments, credit data, and monthly bill statements. The information was based on some people in Taiwan from April 2005 to September 2005.

The variable that was targeted was the default.payment.next.month, where 1 = default and 0 = not defaulted, which was based solely on if they defaulted or not in October of 2005. The 24 features included how much the client owed each month, what the client's payment status was, and the amount paid by the client for each month.

This given dataset simulated a real world situation as the dataset had inaccurate labels for default payment next month, the target variable, the payment status and was also, not precleaned. To further complicate the dataset, it was not clearly explained how to read the dataset correctly and this had to be thoroughly investigated. If you wish to see what each variable means and how they were properly implemented into our model, please check the juypter [file](https://github.com/Zexes9/Credit-Card-Default/blob/main/Default%20of%20credit%20card%20clients.ipynb).

## Methods:
The methodology used was to conduct an EDA, clean the dataset, and the creation of multiple models to see which one would estimate recall best.

## Results:
A Gaussian Naive Bayes model was chosen as it had the best recall prediction score with a value of 89%. Recall was chosen as the benchmark as it was more prudent to predict which customers are likely to have default payments next month or not, rather than overestimate the potential income flow. This would be vital for a bank or credit card company as they can not risk disruption of their cash flow control and risk management. Therefore, it was more important to identify as many potential default customers as possible, even though some of them did not actually default.

### Based the EDA some key finds were found:

Three variables had the highest correlation if a person would default in October or not.
  * They had defaulted in August
  * If they were male
  * Their education level was high school level

## Conclusion:

The bank should be watchful of males, who have defaulted two months prior to the evaluated month and they have a high school education level, as they are more likely to default then others.

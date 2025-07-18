
# 💳  Project Detect Fraud  🏦
Creating a comprehensive ML pipeline to achieve non-zero precision, recall and sensitivity based on historic fraudulent activity.


## Tech Stack

 - Python (`pandas`,`numpy` ,`seaborn` ,`matplotlib`)

- Jupyter Notebook & Markdown

## Goals
 - Form a hypothesis through EDA Analysis
 - Complete data pre-processing
 - Conclude with model generation and hyperparameter search 
## 📘 Data Dictionary 📘 
The descriptions for the each columns of the dataset (categorical and numerical variables) is listed below: 

### Selected Columns

| Column                  | Description                                             |
|-------------------------|---------------------------------------------------------|
| `Type`                  |    The type of transaction                              |
| `Amount`                | The amount of money transferred                      |
| `NameOrig`              |  The origin account name                                |
| `OldBalanceOrg`         | The origin accounts balance before the transaction                                                                         |
| `NewBalanceOrig`        | The origin accounts balance after the transaction                                                                         |
| `NameDest`              | The destination account name                            |
| `OldbalanceDest`        |The destination accounts balance before the transaction                                                                         |
| `NewbalanceDest`        | The destination accounts balance after the transaction                                                                         | 
| `IsFlaggedFraud`*        | A “naive” model that simply flags a transaction as fraudulent if it is greater than 200,000                                                       |
| `IsFraud`              | Was this simulated transaction actually fraudulent? (This will be your target variable)                                                               |

* Note: This currency is not USD

### Dataset Context

The dataset was created to answer the following analytical questions: 

**Exploratory Data Analysis**
- Based on the numberic features in your dataset,how are these values distributed and what might this tell you about how most transactions behave compared to a few rare ones?
- When comparing different numerical features against one another, do any interesting patterns emerge for transactions marked as fraudulent? Are there particular regions or ranges where these transactions seem to concentrate?
- How do types of transaction relate to the typical amounts involved? Are some types of transactions consistently larger or smaller than others?
- Do transaction amounts vary when you compare fraudulent and non-fraudulent transactions across different transaction types? What patterns emerge when you look at both fraud status and transaction type together?
- Consider how well the system's built-in fraud flag (`IsFlaggedFraud`) aligns with actual fraudulent activity. Are there mismatches? What does this tell you about the system's current performance?

**Data Transformation**
 - Does your model contain any missing values or "non-predictive" columns? If so, which adjustments should you take to ensure that your model has good predictive capabilities?
 - Do certain transaction types consistently differ in amount or fraud likelihood? If so, how might you transform the type column to make this pattern usable by a machine learning model?
  - After exploring your data, you may have noticed that fraudulent transactions are rare compared to non-fraudulent ones. What challenges might this pose when training a machine learning model? What strategies could you use to ensure your model learns meaningful patterns from the minority class?
  - Are there interaction effects between variables (e.g., fraud and high amount and transaction type) that aren't captured directly in the dataset? Would it be helpful to manually engineer any new features that reflect these interactions?
   - Are there interaction effects between variables (e.g., fraud and high amount and transaction type) that aren't captured directly in the dataset? Would it be helpful to manually engineer any new features that reflect these interactions?


**Model Selection**
 - Is this a classification or regression task?
- Are you predicting for multiple classes or binary classes?
- Given these observations, which 2 (or possibly 3) machine learning models will you choose?



## Authors

- [@Darylisha Williams](https://github.com/dwilliams170)


## License

[The Knowledge House](https://www.theknowledgehouse.org/) provided the project instructions and raw data for this detect fraud project. 


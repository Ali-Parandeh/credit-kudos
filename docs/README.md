INCOME CLASSIFICATION	

This task is designed to test your ability to apply data science techniques to anonymised Open Banking data. 
You are provided with data.csv, which contains the following fields:

transaction_id: integer ID of the transaction
group_id: integer group ID of the transaction. Transactions in a group will be from the same merchant or individual.
booked_at: date/time that the transactions took place
amount: the transaction value in pence (GBP). For example, 1000 = £10.00. All transactions are credit transactions.
category: a category assigned at a group level.

Transactions would ordinarily contain descriptions, but we have removed them. Your task is to build a classification model which can classify 
groups of credit transactions into the following categories: 'income', or 'other'. Code should be written in Python.

'Income' in this context refers to credit transactions which are in exchange for labor or services, usually from an employer. Similar terms to 
describe income in this context might be 'salary', 'earnings' or 'wages'. We ultimately use these payments to help measure affordability.
Income payments are not for example: credit bank transfers from friends or family, or refunds, which would be labelled as 'other'. 

You should evaluate your model after training. You will be expected to present your model and feature 
selection/extraction methods during a follow-up interview, ideally via a Jupyter notebook.
